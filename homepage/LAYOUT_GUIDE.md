# LiBRE Homepage — Hub Layout Guide

GitHub Pages base URL:
`https://lbhousing.github.io/ArcGIS-Hub`

---

## Hub Page Settings

Set the Hub page **background color to `#0a0e1a`** (near black) so the dark iframe content blends seamlessly. In Hub's page editor, click the page background and enter this hex code.

Set **section backgrounds** to the same `#0a0e1a` unless noted otherwise.

---

## Layout: Row by Row

### ROW 1 — Hero (GitHub iframe)
**Hub element:** Iframe card, full width, NO padding
```
Iframe URL:  https://lbhousing.github.io/ArcGIS-Hub/homepage/hero.html
Height:      700
Scrolling:   no
Frameborder: 0
```
**Hub section settings:** Background `#0a0e1a`, zero padding top/bottom

---

### ROW 2 — Marquee ticker (GitHub iframe)
**Hub element:** Iframe card, full width
```
Iframe URL:  https://lbhousing.github.io/ArcGIS-Hub/homepage/marquee.html
Height:      50
Scrolling:   no
Frameborder: 0
```
**Hub section settings:** Background `#0a0e1a`, zero padding, zero margin

---

### ROW 3 — Stats row (GitHub iframe)
**Hub element:** Iframe card, full width
```
Iframe URL:  https://lbhousing.github.io/ArcGIS-Hub/homepage/stats-row.html
Height:      130
Scrolling:   no
Frameborder: 0
```
**Hub section settings:** Background `#0a0e1a`, padding top 40px, bottom 40px

---

### ROW 4 — Section header "Our Analysis" (Hub text card)
**Hub element:** Text card → Edit in HTML
**Hub section settings:** Background `#0a0e1a`

Paste this HTML:
```html
<div style="padding:20px 0 10px;">
  <div style="font-family:'Segoe UI',system-ui,sans-serif;font-size:72px;font-weight:300;color:#252d4a;line-height:1;">01</div>
  <span style="display:inline-block;font-size:11px;font-weight:600;text-transform:uppercase;letter-spacing:1.5px;padding:5px 14px;border-radius:6px;background:rgba(39,106,219,.12);color:#4d8ae8;border:1px solid rgba(39,106,219,.2);margin-bottom:12px;">Our Analysis</span>
  <h2 style="font-family:'Segoe UI',system-ui,sans-serif;font-size:36px;font-weight:700;color:#f1f5f9;margin:0 0 6px;">Data tools for housing justice.</h2>
  <p style="font-family:'Segoe UI',system-ui,sans-serif;font-size:16px;color:#94a3b8;margin:0;font-weight:300;">Interactive maps, charts, and analysis built from public records — designed for advocates, policymakers, and the renters who deserve to know.</p>
</div>
```

---

### ROW 5 — Page navigation cards (GitHub iframe)
**Hub element:** Iframe card, full width
```
Iframe URL:  https://lbhousing.github.io/ArcGIS-Hub/homepage/page-cards.html
Height:      820
Scrolling:   no
Frameborder: 0
```
Mobile note: Cards stack to 1 column — may need height="1600" on very narrow screens. Test on your phone and adjust. Alternatively, enable `scrolling="auto"`.

**Hub section settings:** Background `#0a0e1a`, padding top 0, bottom 40px

---

### ROW 6 — Divider line (Hub text card)
**Hub element:** Text card → Edit in HTML
**Hub section settings:** Background `#0a0e1a`

```html
<div style="height:1px;background:linear-gradient(90deg,transparent,rgba(255,255,255,.06),transparent);"></div>
```

---

### ROW 7 — Section header "Our Mission" (Hub text card)
**Hub element:** Text card → Edit in HTML
**Hub section settings:** Background `#0a0e1a`

```html
<div style="padding:40px 0 10px;">
  <div style="font-family:'Segoe UI',system-ui,sans-serif;font-size:72px;font-weight:300;color:#252d4a;line-height:1;">02</div>
  <span style="display:inline-block;font-size:11px;font-weight:600;text-transform:uppercase;letter-spacing:1.5px;padding:5px 14px;border-radius:6px;background:rgba(247,186,33,.1);color:#F7BA21;border:1px solid rgba(247,186,33,.2);margin-bottom:12px;">Our Mission</span>
</div>
```

---

### ROW 8 — Mission card (GitHub iframe)
**Hub element:** Iframe card, full width
```
Iframe URL:  https://lbhousing.github.io/ArcGIS-Hub/homepage/mission.html
Height:      340
Scrolling:   no
Frameborder: 0
```
**Hub section settings:** Background `#0a0e1a`, padding bottom 40px

---

### ROW 9 — Divider line (Hub text card)
Same as Row 6.

---

### ROW 10 — Section header "Take Action" (Hub text card)
**Hub element:** Text card → Edit in HTML
**Hub section settings:** Background `#0a0e1a`

```html
<div style="padding:40px 0 10px;">
  <div style="font-family:'Segoe UI',system-ui,sans-serif;font-size:72px;font-weight:300;color:#252d4a;line-height:1;">03</div>
  <span style="display:inline-block;font-size:11px;font-weight:600;text-transform:uppercase;letter-spacing:1.5px;padding:5px 14px;border-radius:6px;background:rgba(210,51,63,.1);color:#D2333F;border:1px solid rgba(210,51,63,.2);margin-bottom:12px;">Take Action</span>
  <h2 style="font-family:'Segoe UI',system-ui,sans-serif;font-size:36px;font-weight:700;color:#f1f5f9;margin:0 0 4px;">Block the Cuts. Build Long Beach.</h2>
  <p style="font-family:'Segoe UI',system-ui,sans-serif;font-size:16px;color:#94a3b8;margin:0;font-weight:300;">LiBRE has joined the LAANE Action Fund and Long Beach Firefighters Local 372 in launching a ballot initiative to protect our city.</p>
</div>
```

---

### ROW 11 — Block the Cuts CTA (GitHub iframe)
**Hub element:** Iframe card, full width
```
Iframe URL:  https://lbhousing.github.io/ArcGIS-Hub/homepage/block-the-cuts.html
Height:      320
Scrolling:   no
Frameborder: 0
```
**Hub section settings:** Background `#0a0e1a`, padding bottom 40px

---

### ROW 12 — Divider line (Hub text card)
Same as Row 6.

---

### ROW 13 — Section header "Resources" (Hub text card)
**Hub element:** Text card → Edit in HTML
**Hub section settings:** Background `#0a0e1a`

```html
<div style="padding:40px 0 10px;">
  <div style="font-family:'Segoe UI',system-ui,sans-serif;font-size:72px;font-weight:300;color:#252d4a;line-height:1;">04</div>
  <span style="display:inline-block;font-size:11px;font-weight:600;text-transform:uppercase;letter-spacing:1.5px;padding:5px 14px;border-radius:6px;background:rgba(52,211,153,.08);color:#34d399;border:1px solid rgba(52,211,153,.2);margin-bottom:12px;">Resources</span>
  <h2 style="font-family:'Segoe UI',system-ui,sans-serif;font-size:36px;font-weight:700;color:#f1f5f9;margin:0 0 4px;">Know your rights as a Long Beach renter.</h2>
  <p style="font-family:'Segoe UI',system-ui,sans-serif;font-size:16px;color:#94a3b8;margin:0;font-weight:300;">Whether or not your building is covered by CTPA, you have protections.</p>
</div>
```

---

### ROW 14 — Know Your Rights cards (GitHub iframe)
**Hub element:** Iframe card, full width
```
Iframe URL:  https://lbhousing.github.io/ArcGIS-Hub/homepage/know-your-rights.html
Height:      200
Scrolling:   no
Frameborder: 0
```
**Hub section settings:** Background `#0a0e1a`, padding bottom 40px

---

### ROW 15 — Footer (GitHub iframe)
**Hub element:** Iframe card, full width
```
Iframe URL:  https://lbhousing.github.io/ArcGIS-Hub/homepage/footer.html
Height:      100
Scrolling:   no
Frameborder: 0
```
**Hub section settings:** Background `#0a0e1a`

---

## Quick Reference

| Row | Type | Content | Height |
|-----|------|---------|--------|
| 1 | iframe | Hero | 700 |
| 2 | iframe | Marquee | 50 |
| 3 | iframe | Stats row | 130 |
| 4 | text card | "01 Our Analysis" header | — |
| 5 | iframe | Page cards (6) | 820 |
| 6 | text card | Divider line | — |
| 7 | text card | "02 Our Mission" header | — |
| 8 | iframe | Mission card | 340 |
| 9 | text card | Divider line | — |
| 10 | text card | "03 Take Action" header | — |
| 11 | iframe | Block the Cuts CTA | 320 |
| 12 | text card | Divider line | — |
| 13 | text card | "04 Resources" header | — |
| 14 | iframe | Know Your Rights (3 cards) | 200 |
| 15 | iframe | Footer | 100 |

**Total: 8 iframes from GitHub + 7 Hub text cards**

---

## GitHub Push Command

From your repo root:
```bash
git add homepage/
git commit -m "Homepage: hero, marquee, stats, page cards, mission, CTA, rights, footer"
git push origin main
```

Pages auto-deploys in ~60 seconds.

---

## Color Reference

All backgrounds: `#0a0e1a`
All text cards must use these text colors to match:
- Headings: `#f1f5f9`
- Body text: `#94a3b8`
- Muted: `#64748b`
- Section numbers: `#252d4a`
- Badges: see individual HTML blocks above
