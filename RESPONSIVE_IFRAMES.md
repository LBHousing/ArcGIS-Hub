# 📐 Responsive iframe heights — READ BEFORE TOUCHING ANY PAGE

**This is the single source of truth for how LiBRE Hub iframes are sized across screen sizes.**
Every page on `weare-libre.hub.arcgis.com` embeds GitHub-hosted HTML "cards" as fixed-height
iframes. Getting the heights wrong is what produces **big empty gaps on mobile** and
**content clipped on desktop** (or vice-versa). Do not skip this doc when editing a page.

---

## The core problem (why this keeps coming back)

1. **ArcGIS Hub iframes have a fixed pixel height** — the content does not auto-resize.
   There is no `pym.js` / no resize script allowed.
2. **Hub lets you set a SEPARATE height for mobile and for desktop.** In the page editor,
   each embed row has a Height field **and** a Mobile Height override. **Both must be set.**
   This is the key fact that was missed before — you are not stuck with one height for both.
3. **Content height changes with width.** A narrative that is 1,868px tall at desktop width
   is 2,573px tall on a phone (text wraps to more lines). A card grid that is 3 columns on
   desktop becomes 1–2 columns on mobile and gets much taller. One height cannot fit both,
   which is *why* Hub gives you two.

### The two failure modes
- **Mobile gap** = mobile height set too **tall** (content is shorter than the box).
- **Desktop clip** = desktop height set too **short** (content is taller than the box).

---

## The rule

For **every** iframe on **every** page, set **two** Hub heights:

- **Mobile Height** = the card's content height at ~**360–390px** wide.
- **Desktop Height** = the card's content height at ~**1140–1200px** wide.

Use the measured tables at the bottom of this doc. When you add or change a card, **re-measure**
(procedure below) and update both this doc and the Hub.

### Observed real iframe widths (do not assume 375/1440)
The Hub does **not** render iframes at the device width. Measured on the live site:

| context | mobile iframe width | desktop iframe width |
|---|---|---|
| full-bleed rows | **390** | **1200** |
| boxed / margin rows (hero, "coming soon", eviction cards) | **360** | **1140** |

Always measure at the width that matches the row type.

---

## Component CSS standard (what each card's HTML must do)

Two patterns are in use. Both are acceptable; pick by content type.

### A. Charts → flex-fill (preferred for anything with a `<canvas>`)
The chart stretches to fill whatever height the iframe is, at any width — so it never gaps or
clips and is forgiving of device-width variation. `build/` (CTPA) and `stats/` charts use this.

```html
<style>
html,body{height:100%}
body{margin:0;overflow:hidden;display:flex;flex-direction:column;padding:14px 28px}
.grid{flex:1 1 auto;min-height:0;display:grid;grid-template-columns:1fr 1fr;grid-auto-rows:1fr;gap:20px}
.card{display:flex;flex-direction:column;min-height:0}     /* card is a flex column */
.cw{position:relative;width:100%;flex:1 1 auto;min-height:0} /* chart wrapper fills the card */
@media(max-width:700px){.grid{grid-template-columns:1fr}}   /* stack on mobile */
</style>
<!-- Chart.js must use: options:{ responsive:true, maintainAspectRatio:false } -->
```
Because it fills, you can even use the **same** height for mobile and desktop. Give mobile a
bit more room (stacked charts) and desktop a bit less (side-by-side).

### B. Text / card grids → natural flow, set two heights
Prose and stat-card grids can't "fill" gracefully, so let them flow at their natural height and
set the two Hub heights to the measured content height at each width.

**Hard rules for every card, both patterns:**
- **No horizontal overflow.** Any decorative absolutely-positioned element (e.g. `.hero::before`
  glow blobs at `right:-200px`) MUST be clipped by `overflow:hidden` on its container, or it
  adds ~200px of sideways scroll that cuts content off on mobile. *(This bug was found on 5 hero
  cards and fixed — see git history.)*
- Use `padding` in `%`/`px` that shrinks on mobile via `@media`.
- Test at 360, 390, 1140, and 1200 before shipping.

---

## Measurement procedure (run this whenever a card changes)

From `capture_tool/` (has Playwright + Chromium in `node_modules`):

```js
// _measure.js  —  node _measure.js
const { chromium } = require('playwright');
const FILE = 'c:/Users/Zoro/Documents/LiBRE/ArcGIS-Hub/<folder>/<card>.html';
(async () => {
  const b = await chromium.launch();
  for (const [tag, w] of [['MOBILE', 390], ['DESKTOP', 1200]]) {   // use 360/1140 for boxed rows
    const c = await b.newContext({ viewport: { width: w, height: 400 } });
    const p = await c.newPage();
    await p.goto('file:///' + FILE, { waitUntil: 'networkidle' });
    await p.waitForTimeout(900);
    const r = await p.evaluate(() => {
      const de = document.documentElement, bd = document.body;
      de.style.setProperty('height','auto','important');          // un-clamp natural-flow cards
      bd.style.setProperty('height','auto','important');
      bd.style.setProperty('overflow','visible','important');
      return { h: Math.max(bd.scrollHeight, de.scrollHeight),
               overflowX: de.scrollWidth - window.innerWidth };    // must be 0
    });
    console.log(tag, 'set height ≈', r.h + 20, ' | horizontal overflow:', r.overflowX);
    await c.close();
  }
  await b.close();
})();
```
- **Set the Hub height to the reported value** (already includes a ~20px buffer).
- **`horizontal overflow` must be 0.** If not, add `overflow:hidden` to the offending container.
- Flex-fill chart cards report a floor value (they fill any height) — pick a sensible height
  instead of measuring; the tables below already list good ones.

---

## Per-page height tables (measured Aug 2026)

`M` = Mobile Height, `D` = Desktop Height (pixels to enter in the Hub). `flex` = flex-fill chart
(forgiving). Marquees are thin scrollers — leave as-is.

### Home — `/` → repo `homepage/`
| card | M | D | notes |
|---|---|---|---|
| hero | 640 | 660 | overflow bug fixed |
| marquee | 50 | 50 | |
| mission | 900 | 540 | |
| stats-row | 130 | 130 | |
| block-the-cuts | 580 | 440 | |
| page-cards | 1560 | 660 | tall on mobile (cards stack) |
| know-your-rights | 540 | 440 | |

### District Stats — `/pages/district-stats` → repo `stats/`
| card | M | D | notes |
|---|---|---|---|
| hero | 960 | 740 | overflow bug fixed |
| marquee (citywide) | 50 | 50 | |
| metrics | 1180 | 1020 | 2-col both widths |
| charts-all-renters | 500 | 400 | flex |
| charts-seniors | 500 | 400 | flex |
| charts-lowincome | 500 | 400 | flex |
| marquee-districts | 50 | 50 | |
| district-bars | 840 | 560 | flex (3 charts) |
| district-cards | 1160 | 1060 | 2-col both widths |
| narr-analysis | 2610 | 1900 | long essay; can't fully converge |

### Ownership / CTPA — `/pages/ctpa` → repo `build/`
Flex-fill design — the same height works for **both** M and D. Values from `build/README.md`.
| card | M | D | notes |
|---|---|---|---|
| hero | 683 | 683 | flex |
| marquee | 56 | 56 | |
| metric-bars | 312 | 312 | |
| charts-ownership | 660 | 660 | flex |
| formshift-tiles | 180 | 162 | tiles stack on mobile |
| formshift-chart | 560 | 540 | flex |
| narr-shift | 740 | 701 | |
| metric-trusts | 220 | 160 | bars stack on mobile |
| narr-trusts | 560 | 550 | |
| concentration | 940 | 907 | flex + narrative |
| builders | 1400 | 1240 | |
| acquisition | 1280 | 1400 | desktop taller (2-col cards) |
| chart-top25 | 900 | 900 | flex |
| buildcase | 1120 | 940 | |
| narr-protections | 930 | 900 | |
| charts-historical | 680 | 660 | flex |
| know-your-rights | 560 | 460 | |

### Housing Maps — `/pages/housing-maps` → repo `conditions/`
| card | M | D | notes |
|---|---|---|---|
| hero | 540 | 620 | overflow bug fixed |
| marquee | 50 | 50 | |
| timeline | 3300 | 1680 | very tall on mobile |
| narr-violations | 860 | 440 | |
| narr-evictions | 890 | 440 | |
| action-cards | 980 | 440 | |
| narr-demographics | 950 | 440 | |

### Evictions — `/pages/eviction-analysis` → repo `eviction-dashboard/cards/…` + `eviction-coming-soon.html`
Boxed rows → measured at 360 / 1140.
| card | M | D | notes |
|---|---|---|---|
| eviction-coming-soon | 520 | 460 | overflow bug fixed |
| eviction-map | 1080 | 800 | |
| headline-numbers | 880 | 440 | |
| funnel | 240 | 240 | |
| owner-type | 540 | 440 | |
| top-filers | 560 | 740 | desktop taller |
| trend | 560 | 520 | |
| cohort | 580 | 480 | |
| seasonality | 500 | 460 | |
| policy-impact | 880 | 440 | |
| data-quality | 640 | 440 | |

### Our Team — `/pages/our-team` → repo `libre-team/`
| card | M | D | notes |
|---|---|---|---|
| hero | 660 | 580 | overflow bug fixed |
| marquee | 60 | 60 | |
| partners | 1620 | 670 | tall on mobile |
| team-cards | 730 | 440 | |
| collabs | 820 | 440 | |
| dslc | 3560 | 1650 | very tall; desktop currently clips |
| origins | 1280 | 590 | |
| updates-bar | 240 | 240 | |

---

## Checklist when adding or editing any card
- [ ] Component CSS: charts flex-fill (pattern A) or text flows naturally (pattern B).
- [ ] `overflow:hidden` on any container with decorative absolutely-positioned children.
- [ ] Run the measurement script at the row's real widths (360/390 mobile, 1140/1200 desktop).
- [ ] `horizontal overflow` reads 0 at both widths.
- [ ] Enter **both** the Mobile Height and Desktop Height in the Hub row.
- [ ] Update the table above with the new numbers.
