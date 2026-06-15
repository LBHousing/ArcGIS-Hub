# Block the Cuts & Build LB: "Who Owns Long Beach" Hub Layout Guide

**Updated build:** consolidated 2018-2026 Assessor analysis, dwelling-units only.
Replace `BASEURL` with: `https://lbhousing.github.io/ArcGIS-Hub`
All Hub section backgrounds: `#0a0e1a`

Each `build/*.html` file is a self-contained iframe (its own fonts + Chart.js).
Section headers and dividers are native **Hub text cards** (paste the HTML).
Heights below include a small buffer; nudge ±20px to taste.

---

## Row-by-Row Assembly

### ROW 1 — Hero (iframe)
```
URL:    BASEURL/build/hero.html
Height: 540
```

### ROW 2 — Marquee (iframe)
```
URL:    BASEURL/build/marquee.html
Height: 56
```

### ROW 3 — Section header "Citywide Ownership" (text card)
```html
<div style="padding:40px 0 10px;">
  <span style="display:inline-block;font-size:11px;font-weight:600;text-transform:uppercase;letter-spacing:1.5px;padding:5px 14px;border-radius:6px;background:rgba(39,106,219,.12);color:#4d8ae8;border:1px solid rgba(39,106,219,.2);margin-bottom:12px;">Citywide Ownership</span>
  <h2 style="font-family:'Segoe UI',system-ui,sans-serif;font-size:36px;font-weight:700;color:#f1f5f9;margin:0 0 6px;">Every parcel. Every owner type. The full picture.</h2>
  <p style="font-family:'Segoe UI',system-ui,sans-serif;font-size:16px;color:#94a3b8;margin:0;font-weight:300;">All 177,588 dwelling units in Long Beach, by who holds title in 2026, and how each category shifted since 2018.</p>
</div>
```

### ROW 4 — Metric bars, 6 owner types (iframe)
```
URL:    BASEURL/build/metric-bars.html
Height: 300
```

### ROW 5 — Ownership charts: donut + nine-year change (iframe)
```
URL:    BASEURL/build/charts-ownership.html
Height: 440
```

### ROW 6 — Divider (text card)
```html
<div style="height:1px;background:linear-gradient(90deg,transparent,rgba(255,255,255,.06),transparent);"></div>
```

### ROW 7 — Section header "The Form Shift" (text card)
```html
<div style="padding:40px 0 10px;">
  <span style="display:inline-block;font-size:11px;font-weight:600;text-transform:uppercase;letter-spacing:1.5px;padding:5px 14px;border-radius:6px;background:rgba(210,51,63,.1);color:#D2333F;border:1px solid rgba(210,51,63,.2);margin-bottom:12px;">The Form Shift</span>
  <h2 style="font-family:'Segoe UI',system-ui,sans-serif;font-size:36px;font-weight:700;color:#f1f5f9;margin:0 0 6px;">The housing didn't disappear. The owners changed shape.</h2>
  <p style="font-family:'Segoe UI',system-ui,sans-serif;font-size:16px;color:#94a3b8;margin:0;font-weight:300;">Long Beach's rental stock grew by just +4,277 units in nine years. The legal form of ownership shifted away from people toward entities.</p>
</div>
```

### ROW 8 — Form-shift stat tiles (iframe)
```
URL:    BASEURL/build/formshift-tiles.html
Height: 150
```

### ROW 9 — Form-shift chart: 100% stacked area (iframe)
```
URL:    BASEURL/build/formshift-chart.html
Height: 540
```

### ROW 10 — Shift narrative (iframe)
```
URL:    BASEURL/build/narr-shift.html
Height: 340
```

### ROW 11 — Divider (text card)
```html
<div style="height:1px;background:linear-gradient(90deg,transparent,rgba(255,255,255,.06),transparent);"></div>
```

### ROW 12 — Section header "The Trust Loophole" (text card)
```html
<div style="padding:40px 0 10px;">
  <span style="display:inline-block;font-size:11px;font-weight:600;text-transform:uppercase;letter-spacing:1.5px;padding:5px 14px;border-radius:6px;background:rgba(123,78,175,.1);color:#9d6fc7;border:1px solid rgba(123,78,175,.2);margin-bottom:12px;">The Trust Loophole</span>
  <h2 style="font-family:'Segoe UI',system-ui,sans-serif;font-size:36px;font-weight:700;color:#f1f5f9;margin:0 0 6px;">Individual trusts get homeowner treatment even at institutional scale.</h2>
  <p style="font-family:'Segoe UI',system-ui,sans-serif;font-size:16px;color:#94a3b8;margin:0;font-weight:300;">2,929 trusts own multiple properties; 139 average 25 units each.</p>
</div>
```

### ROW 13 — Trust metric bars, 3 (iframe)
```
URL:    BASEURL/build/metric-trusts.html
Height: 160
```

### ROW 14 — Trust narrative (iframe)
```
URL:    BASEURL/build/narr-trusts.html
Height: 340
```

### ROW 15 — Divider (text card)
```html
<div style="height:1px;background:linear-gradient(90deg,transparent,rgba(255,255,255,.06),transparent);"></div>
```

### ROW 16 — Section header "Ownership Concentration" (text card)
```html
<div style="padding:40px 0 10px;">
  <span style="display:inline-block;font-size:11px;font-weight:600;text-transform:uppercase;letter-spacing:1.5px;padding:5px 14px;border-radius:6px;background:rgba(210,51,63,.1);color:#D2333F;border:1px solid rgba(210,51,63,.2);margin-bottom:12px;">Ownership Concentration</span>
  <h2 style="font-family:'Segoe UI',system-ui,sans-serif;font-size:36px;font-weight:700;color:#f1f5f9;margin:0 0 6px;">A few owners hold a lot, but the very top isn't getting bigger.</h2>
  <p style="font-family:'Segoe UI',system-ui,sans-serif;font-size:16px;color:#94a3b8;margin:0;font-weight:300;">5,368 multi-property owners control 44,107 units (24.8% of the city). The largest owners' share has stayed flat since 2018.</p>
</div>
```

### ROW 17 — Concentration chart + narrative (iframe)
```
URL:    BASEURL/build/concentration.html
Height: 520
```

### ROW 18 — Divider (text card)
```html
<div style="height:1px;background:linear-gradient(90deg,transparent,rgba(255,255,255,.06),transparent);"></div>
```

### ROW 19 — Section header "The Builders" (text card)
```html
<div style="padding:40px 0 10px;">
  <span style="display:inline-block;font-size:11px;font-weight:600;text-transform:uppercase;letter-spacing:1.5px;padding:5px 14px;border-radius:6px;background:rgba(52,211,153,.08);color:#34d399;border:1px solid rgba(52,211,153,.2);margin-bottom:12px;">The Builders</span>
  <h2 style="font-family:'Segoe UI',system-ui,sans-serif;font-size:36px;font-weight:700;color:#f1f5f9;margin:0 0 6px;">The biggest gainers built new housing, split evenly between market-rate and affordable.</h2>
  <p style="font-family:'Segoe UI',system-ui,sans-serif;font-size:16px;color:#94a3b8;margin:0;font-weight:300;">The ten owners who added the most units weren't buying up the city. They were building it, half luxury and half affordable. Every affordable project needed public money.</p>
</div>
```

### ROW 20 — The Builders: market/affordable split + 10 cards (iframe)
```
URL:    BASEURL/build/builders.html
Height: 1200
```

### ROW 21 — Divider (text card)
```html
<div style="height:1px;background:linear-gradient(90deg,transparent,rgba(255,255,255,.06),transparent);"></div>
```

### ROW 22 — Section header "The Quiet Acquisition" (text card)
```html
<div style="padding:40px 0 10px;">
  <span style="display:inline-block;font-size:11px;font-weight:600;text-transform:uppercase;letter-spacing:1.5px;padding:5px 14px;border-radius:6px;background:rgba(247,186,33,.1);color:#F7BA21;border:1px solid rgba(247,186,33,.2);margin-bottom:12px;">The Quiet Acquisition</span>
  <h2 style="font-family:'Segoe UI',system-ui,sans-serif;font-size:36px;font-weight:700;color:#f1f5f9;margin:0 0 6px;">Meanwhile, the old, naturally-affordable buildings changed hands.</h2>
  <p style="font-family:'Segoe UI',system-ui,sans-serif;font-size:16px;color:#94a3b8;margin:0;font-weight:300;">1,553 older rental buildings passed from individual owners into LLCs, LPs, and corporations through two paths.</p>
</div>
```

### ROW 23 — The Quiet Acquisition: mechanism + acquirer cards + mobile-home parks (iframe)
```
URL:    BASEURL/build/acquisition.html
Height: 1180
```

### ROW 24 — Divider (text card)
```html
<div style="height:1px;background:linear-gradient(90deg,transparent,rgba(255,255,255,.06),transparent);"></div>
```

### ROW 25 — Section header "Largest Owners" (text card)
```html
<div style="padding:40px 0 10px;">
  <span style="display:inline-block;font-size:11px;font-weight:600;text-transform:uppercase;letter-spacing:1.5px;padding:5px 14px;border-radius:6px;background:rgba(247,186,33,.1);color:#F7BA21;border:1px solid rgba(247,186,33,.2);margin-bottom:12px;">Largest Owners</span>
  <h2 style="font-family:'Segoe UI',system-ui,sans-serif;font-size:36px;font-weight:700;color:#f1f5f9;margin:0 0 6px;">The 25 biggest entity owners in Long Beach.</h2>
  <p style="font-family:'Segoe UI',system-ui,sans-serif;font-size:16px;color:#94a3b8;margin:0;font-weight:300;">The top owner controls 538 units on just 2 parcels. Hotels, storage, and other non-dwellings removed.</p>
</div>
```

### ROW 26 — Top 25 horizontal bar (iframe)
```
URL:    BASEURL/build/chart-top25.html
Height: 900
```

### ROW 27 — Divider (text card)
```html
<div style="height:1px;background:linear-gradient(90deg,transparent,rgba(255,255,255,.06),transparent);"></div>
```

### ROW 28 — Section header "The Build Case" (text card)
```html
<div style="padding:40px 0 10px;">
  <span style="display:inline-block;font-size:11px;font-weight:600;text-transform:uppercase;letter-spacing:1.5px;padding:5px 14px;border-radius:6px;background:rgba(52,211,153,.08);color:#34d399;border:1px solid rgba(52,211,153,.2);margin-bottom:12px;">The Build Case</span>
  <h2 style="font-family:'Segoe UI',system-ui,sans-serif;font-size:36px;font-weight:700;color:#f1f5f9;margin:0 0 6px;">The city is building. Just nowhere near enough.</h2>
</div>
```

### ROW 29 — Build case: ladder + RHNA tiles + CLT pitch (iframe)
```
URL:    BASEURL/build/buildcase.html
Height: 710
```

### ROW 30 — Divider (text card)
```html
<div style="height:1px;background:linear-gradient(90deg,transparent,rgba(255,255,255,.06),transparent);"></div>
```

### ROW 31 — Section header "Renter Protections" (text card)
```html
<div style="padding:40px 0 10px;">
  <span style="display:inline-block;font-size:11px;font-weight:600;text-transform:uppercase;letter-spacing:1.5px;padding:5px 14px;border-radius:6px;background:rgba(39,106,219,.12);color:#4d8ae8;border:1px solid rgba(39,106,219,.2);margin-bottom:12px;">Renter Protections</span>
  <h2 style="font-family:'Segoe UI',system-ui,sans-serif;font-size:36px;font-weight:700;color:#f1f5f9;margin:0 0 6px;">What this means for tenant protections.</h2>
</div>
```

### ROW 32 — Protections narrative (iframe)
```
URL:    BASEURL/build/narr-protections.html
Height: 540
```

### ROW 33 — Divider (text card)
```html
<div style="height:1px;background:linear-gradient(90deg,transparent,rgba(255,255,255,.06),transparent);"></div>
```

### ROW 34 — Section header "Historical Context" (text card)
```html
<div style="padding:40px 0 10px;">
  <span style="display:inline-block;font-size:11px;font-weight:600;text-transform:uppercase;letter-spacing:1.5px;padding:5px 14px;border-radius:6px;background:rgba(39,106,219,.12);color:#4d8ae8;border:1px solid rgba(39,106,219,.2);margin-bottom:12px;">Historical Context</span>
  <h2 style="font-family:'Segoe UI',system-ui,sans-serif;font-size:36px;font-weight:700;color:#f1f5f9;margin:0 0 6px;">Flat housing supply. Soaring value.</h2>
  <p style="font-family:'Segoe UI',system-ui,sans-serif;font-size:16px;color:#94a3b8;margin:0;font-weight:300;">Long Beach added almost no net housing, yet assessed value climbed from $41.6B to $63.3B.</p>
</div>
```

### ROW 35 — Historical value charts, 2 (iframe)
```
URL:    BASEURL/build/charts-historical.html
Height: 420
```

### ROW 36 — Divider (text card)
```html
<div style="height:1px;background:linear-gradient(90deg,transparent,rgba(255,255,255,.06),transparent);"></div>
```

### ROW 37 — Section header "Know Your Rights" (text card)
```html
<div style="padding:40px 0 10px;">
  <span style="display:inline-block;font-size:11px;font-weight:600;text-transform:uppercase;letter-spacing:1.5px;padding:5px 14px;border-radius:6px;background:rgba(52,211,153,.08);color:#34d399;border:1px solid rgba(52,211,153,.2);margin-bottom:12px;">Know Your Rights</span>
  <h2 style="font-family:'Segoe UI',system-ui,sans-serif;font-size:36px;font-weight:700;color:#f1f5f9;margin:0 0 6px;">You may have more protection than you think.</h2>
</div>
```

### ROW 38 — Know Your Rights resources (iframe)
```
URL:    BASEURL/build/know-your-rights.html
Height: 390
```

---

## Quick Reference

| Row | Type | Content | Height |
|-----|------|---------|--------|
| 1 | iframe | Hero + counters | 540 |
| 2 | iframe | Marquee | 56 |
| 3 | text card | Citywide Ownership | n/a |
| 4 | iframe | Metric bars (6) | 300 |
| 5 | iframe | Donut + nine-year change | 440 |
| 6 | text card | Divider | n/a |
| 7 | text card | The Form Shift | n/a |
| 8 | iframe | Form-shift tiles (3) | 150 |
| 9 | iframe | Stacked-area chart | 540 |
| 10 | iframe | Shift narrative | 340 |
| 11 | text card | Divider | n/a |
| 12 | text card | The Trust Loophole | n/a |
| 13 | iframe | Trust metric bars (3) | 160 |
| 14 | iframe | Trust narrative | 340 |
| 15 | text card | Divider | n/a |
| 16 | text card | Ownership Concentration | n/a |
| 17 | iframe | Concentration chart + narrative | 520 |
| 18 | text card | Divider | n/a |
| 19 | text card | The Builders | n/a |
| 20 | iframe | Builders split + 10 cards | 1200 |
| 21 | text card | Divider | n/a |
| 22 | text card | The Quiet Acquisition | n/a |
| 23 | iframe | Acquisition + acquirers + MHP | 1180 |
| 24 | text card | Divider | n/a |
| 25 | text card | Largest Owners | n/a |
| 26 | iframe | Top 25 horizontal bar | 900 |
| 27 | text card | Divider | n/a |
| 28 | text card | The Build Case | n/a |
| 29 | iframe | Build-case ladder + tiles | 710 |
| 30 | text card | Divider | n/a |
| 31 | text card | Renter Protections | n/a |
| 32 | iframe | Protections narrative | 540 |
| 33 | text card | Divider | n/a |
| 34 | text card | Historical Context | n/a |
| 35 | iframe | Historical charts (2) | 420 |
| 36 | text card | Divider | n/a |
| 37 | text card | Know Your Rights | n/a |
| 38 | iframe | Know Your Rights | 390 |

**Total: 17 GitHub iframes + 11 section headers + 10 dividers**

---

## What changed from the previous build

- **New sections:** The Form Shift (tiles + stacked-area), The Builders, The Quiet Acquisition, The Build Case.
- **New files:** `formshift-tiles.html`, `formshift-chart.html`, `builders.html`, `acquisition.html`, `buildcase.html`, `concentration.html` (chart + narrative combined).
- **Replaced:** `chart-concentration.html` is superseded by `concentration.html`. `charts-owner-type.html` is retired; its 2023-vs-2025 bars are covered by the nine-year stacked-area chart. Both old files are kept as archive.
- **Data:** rebuilt on the parcel-level 2018-2026 Assessor roll, **dwelling units only** (hotels, motels, self-storage, cemeteries, churches, schools, medical, retail, and office excluded). Headline 2026 figures: 177,588 units / 98,396 parcels; entity-controlled 25.9%; LLCs +11,148 (54.6%) since 2018.

---

## GitHub Push Command

```bash
git add build/
git commit -m "Who Owns LB: consolidated 2018-2026 dwelling-only build (17 cards + layout)"
git push origin main
```

---

## Full Repo Structure After This Push

```
ArcGIS-Hub/
├── home/          <- Homepage
├── charts/        <- District Statistics charts
├── districts/     <- District cards D1-D9
├── conditions/    <- Housing Conditions
├── build/         <- Who Owns LB (17 iframe cards + this README)
└── README.md
```
