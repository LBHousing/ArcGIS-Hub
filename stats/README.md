# District Statistics Page — Hub Layout Guide

Replace `BASEURL` with: `https://lbhousing.github.io/ArcGIS-Hub`

All Hub section backgrounds: `#0a0e1a`

---

## Row-by-Row Assembly

### ROW 1 — Hero (GitHub iframe)
```
URL:    BASEURL/stats/hero.html
Height: 800
```
3 rows of stats (12 indicators) with numbered footnotes. Sources: Census ACS, NLIHC, Long Beach Forward, USC Lusk Center.

### ROW 2 — Marquee (GitHub iframe)
```
URL:    BASEURL/stats/marquee.html
Height: 50
```

### ROW 3 — Section header "Citywide Snapshot" (Hub text card)
```html
<div style="padding:40px 0 10px;">
  <div style="font-family:'Segoe UI',system-ui,sans-serif;font-size:80px;font-weight:300;color:#252d4a;line-height:1;">01</div>
  <span style="display:inline-block;font-size:11px;font-weight:600;text-transform:uppercase;letter-spacing:1.5px;padding:5px 14px;border-radius:6px;background:rgba(39,106,219,.12);color:#4d8ae8;border:1px solid rgba(39,106,219,.2);margin-bottom:12px;">Citywide Snapshot</span>
  <h2 style="font-family:'Segoe UI',system-ui,sans-serif;font-size:36px;font-weight:700;color:#f1f5f9;margin:0 0 6px;">Long Beach housing at a glance.</h2>
  <p style="font-family:'Segoe UI',system-ui,sans-serif;font-size:16px;color:#94a3b8;margin:0;font-weight:300;">Key indicators from the 2020-2024 ACS with 10-year trends from 2010-2014.</p>
</div>
```

### ROW 4 — Metric bars — expanded (GitHub iframe)
```
URL:    BASEURL/stats/metrics.html
Height: 540
```
12 metric cards in 3 rows of 4, grouped by category (All Renters / Seniors / Low-Income) with colored section labels and dividers between groups.

### ROW 5 — Divider (Hub text card)
```html
<div style="height:1px;background:linear-gradient(90deg,transparent,rgba(255,255,255,.06),transparent);"></div>
```

### ROW 6 — Section header "All Renters" (Hub text card)
```html
<div style="padding:40px 0 10px;">
  <div style="font-family:'Segoe UI',system-ui,sans-serif;font-size:80px;font-weight:300;color:#252d4a;line-height:1;">02</div>
  <span style="display:inline-block;font-size:11px;font-weight:600;text-transform:uppercase;letter-spacing:1.5px;padding:5px 14px;border-radius:6px;background:rgba(39,106,219,.12);color:#4d8ae8;border:1px solid rgba(39,106,219,.2);margin-bottom:12px;">B25070 — All Renters</span>
  <h2 style="font-family:'Segoe UI',system-ui,sans-serif;font-size:36px;font-weight:700;color:#f1f5f9;margin:0 0 6px;">Total rent burden households.</h2>
  <p style="font-family:'Segoe UI',system-ui,sans-serif;font-size:16px;color:#94a3b8;margin:0;font-weight:300;">Tracking the percentage of all renter households spending 30%+ of income on housing.</p>
</div>
```

### ROW 7 — All renters charts (GitHub iframe)
```
URL:    BASEURL/stats/charts-all-renters.html
Height: 400
```

### ROW 8 — Divider (Hub text card)

### ROW 9 — Section header "Seniors" (Hub text card)
```html
<div style="padding:40px 0 10px;">
  <div style="font-family:'Segoe UI',system-ui,sans-serif;font-size:80px;font-weight:300;color:#252d4a;line-height:1;">03</div>
  <span style="display:inline-block;font-size:11px;font-weight:600;text-transform:uppercase;letter-spacing:1.5px;padding:5px 14px;border-radius:6px;background:rgba(123,78,175,.1);color:#7B4EAF;border:1px solid rgba(123,78,175,.2);margin-bottom:12px;">B25072 — Senior Renters</span>
  <h2 style="font-family:'Segoe UI',system-ui,sans-serif;font-size:36px;font-weight:700;color:#f1f5f9;margin:0 0 6px;">Rent-burdened households 65+.</h2>
  <p style="font-family:'Segoe UI',system-ui,sans-serif;font-size:16px;color:#94a3b8;margin:0;font-weight:300;">Seniors on fixed incomes are among the most vulnerable to housing cost increases.</p>
</div>
```

### ROW 10 — Senior charts (GitHub iframe)
```
URL:    BASEURL/stats/charts-seniors.html
Height: 400
```

### ROW 11 — Divider (Hub text card)

### ROW 12 — Section header "Low-Income" (Hub text card)
```html
<div style="padding:40px 0 10px;">
  <div style="font-family:'Segoe UI',system-ui,sans-serif;font-size:80px;font-weight:300;color:#252d4a;line-height:1;">04</div>
  <span style="display:inline-block;font-size:11px;font-weight:600;text-transform:uppercase;letter-spacing:1.5px;padding:5px 14px;border-radius:6px;background:rgba(247,186,33,.1);color:#F7BA21;border:1px solid rgba(247,186,33,.2);margin-bottom:12px;">B25074 — Low-Income Renters</span>
  <h2 style="font-family:'Segoe UI',system-ui,sans-serif;font-size:36px;font-weight:700;color:#f1f5f9;margin:0 0 6px;">Low-income households severely burdened.</h2>
  <p style="font-family:'Segoe UI',system-ui,sans-serif;font-size:16px;color:#94a3b8;margin:0;font-weight:300;">Households under $35K face the most acute pressure. Declining counts signal displacement.</p>
</div>
```

### ROW 13 — Low-income charts (GitHub iframe)
```
URL:    BASEURL/stats/charts-lowincome.html
Height: 400
```

### ROW 14 — Divider (Hub text card)

### ROW 15 — District marquee (GitHub iframe)
```
URL:    BASEURL/stats/marquee-districts.html
Height: 50
```
Color-coded scrolling ticker showing the highest-burden districts — creates a visual break before the bar charts.

### ROW 16 — Section header "District Comparison" (Hub text card)
```html
<div style="padding:40px 0 10px;">
  <div style="font-family:'Segoe UI',system-ui,sans-serif;font-size:80px;font-weight:300;color:#252d4a;line-height:1;">05</div>
  <span style="display:inline-block;font-size:11px;font-weight:600;text-transform:uppercase;letter-spacing:1.5px;padding:5px 14px;border-radius:6px;background:rgba(210,51,63,.1);color:#D2333F;border:1px solid rgba(210,51,63,.2);margin-bottom:12px;">By Council District</span>
  <h2 style="font-family:'Segoe UI',system-ui,sans-serif;font-size:36px;font-weight:700;color:#f1f5f9;margin:0 0 6px;">Not all districts face the same burden.</h2>
  <p style="font-family:'Segoe UI',system-ui,sans-serif;font-size:16px;color:#94a3b8;margin:0;font-weight:300;">Districts above the citywide average are highlighted in red.</p>
</div>
```

### ROW 16 — Section header "District Comparison" (Hub text card)
```html
<div style="padding:40px 0 10px;">
  <div style="font-family:'Segoe UI',system-ui,sans-serif;font-size:80px;font-weight:300;color:#252d4a;line-height:1;">05</div>
  <span style="display:inline-block;font-size:11px;font-weight:600;text-transform:uppercase;letter-spacing:1.5px;padding:5px 14px;border-radius:6px;background:rgba(210,51,63,.1);color:#D2333F;border:1px solid rgba(210,51,63,.2);margin-bottom:12px;">By Council District</span>
  <h2 style="font-family:'Segoe UI',system-ui,sans-serif;font-size:36px;font-weight:700;color:#f1f5f9;margin:0 0 6px;">Not all districts face the same burden.</h2>
  <p style="font-family:'Segoe UI',system-ui,sans-serif;font-size:16px;color:#94a3b8;margin:0;font-weight:300;">Districts above the citywide average are highlighted in red.</p>
</div>
```

### ROW 17 — District bar charts (GitHub iframe)
```
URL:    BASEURL/stats/district-bars.html
Height: 780
```

### ROW 18 — Divider (Hub text card)

### ROW 19 — Section header "District Breakdown" (Hub text card)
```html
<div style="padding:40px 0 10px;">
  <div style="font-family:'Segoe UI',system-ui,sans-serif;font-size:80px;font-weight:300;color:#252d4a;line-height:1;">06</div>
  <span style="display:inline-block;font-size:11px;font-weight:600;text-transform:uppercase;letter-spacing:1.5px;padding:5px 14px;border-radius:6px;background:rgba(39,106,219,.12);color:#4d8ae8;border:1px solid rgba(39,106,219,.2);margin-bottom:12px;">By Council District</span>
  <h2 style="font-family:'Segoe UI',system-ui,sans-serif;font-size:36px;font-weight:700;color:#f1f5f9;margin:0 0 6px;">Council district breakdown.</h2>
  <p style="font-family:'Segoe UI',system-ui,sans-serif;font-size:16px;color:#94a3b8;margin:0;font-weight:300;">Each district's current indicators with 10-year sparklines.</p>
</div>
```

### ROW 20 — District cards with sparklines (GitHub iframe)
```
URL:    BASEURL/stats/district-cards.html
Height: 620
```
9 compact cards in a 3x3 grid. Each shows burden %, senior burden %, and low-income severe % with mini sparklines and 10-year delta arrows. Above/below average badge per district.

### ROW 21 — Divider (Hub text card)

### ROW 22 — Section header "Analysis" (Hub text card)
```html
<div style="padding:40px 0 10px;">
  <div style="font-family:'Segoe UI',system-ui,sans-serif;font-size:80px;font-weight:300;color:#252d4a;line-height:1;">07</div>
  <span style="display:inline-block;font-size:11px;font-weight:600;text-transform:uppercase;letter-spacing:1.5px;padding:5px 14px;border-radius:6px;background:rgba(52,211,153,.08);color:#34d399;border:1px solid rgba(52,211,153,.2);margin-bottom:12px;">Analysis</span>
  <h2 style="font-family:'Segoe UI',system-ui,sans-serif;font-size:36px;font-weight:700;color:#f1f5f9;margin:0 0 6px;">What the data tells us.</h2>
</div>
```

### ROW 23 — Narrative (GitHub iframe)
```
URL:    BASEURL/stats/narr-analysis.html
Height: 1400
```

### ROW 24 — Source banner (Hub text card)
```html
<div style="background:#111827;border:1px solid rgba(255,255,255,.06);border-radius:8px;padding:12px 20px;text-align:center;font-family:'Segoe UI',system-ui,sans-serif;">
  <p style="font-size:12px;color:#64748b;margin:0;line-height:1.6;">Data: <strong style="color:#94a3b8">U.S. Census Bureau</strong> ACS 5-Year Estimates (Tables B25070, B25072, B25074) | 116 census tracts weighted by council district area overlap | Analysis by <strong style="color:#94a3b8">LiBRE</strong></p>
</div>
```

---

## Quick Reference

| Row | Type | Content | Height |
|-----|------|---------|--------|
| 1 | iframe | Hero + 12 stats + sources | 800 |
| 2 | iframe | Marquee (citywide) | 50 |
| 3 | text card | "01 Citywide Snapshot" | — |
| 4 | iframe | Metric bars (12 cards, 3 categories) | 540 |
| 5 | text card | Divider | — |
| 6 | text card | "02 All Renters" | — |
| 7 | iframe | Rate + count charts | 400 |
| 8 | text card | Divider | — |
| 9 | text card | "03 Seniors" | — |
| 10 | iframe | Rate + count charts | 400 |
| 11 | text card | Divider | — |
| 12 | text card | "04 Low-Income" | — |
| 13 | iframe | Rate + count charts | 400 |
| 14 | text card | Divider | — |
| 15 | iframe | Marquee (district stats) | 50 |
| 16 | text card | "05 District Comparison" | — |
| 17 | iframe | 3 district bar charts | 780 |
| 18 | text card | Divider | — |
| 19 | text card | "06 District Breakdown" | — |
| 20 | iframe | 9 district cards w/ sparklines | 620 |
| 21 | text card | Divider | — |
| 22 | text card | "07 Analysis" | — |
| 23 | iframe | Full narrative | 1400 |
| 24 | text card | Source banner | — |

**Total: 10 GitHub iframes + 14 Hub text cards**

---

## GitHub Push Command

```bash
git add stats/
git commit -m "District Stats dark theme: hero, marquee, metrics, charts, bars, narrative"
git push origin main
```

---

## Color Reference for This Page

| Category | Color | Used for |
|----------|-------|----------|
| All Renters (B25070) | `#276ADB` / `#4d8ae8` | Pyramid blue — charts, badges, text |
| Seniors (B25072) | `#7B4EAF` | Purple — charts, badges |
| Low-Income (B25074) | `#F7BA21` | Poppy yellow — charts, badges |
| Above Average / Worsening | `#D2333F` | Bottlebrush red — district bars, alerts |
| Improving | `#34d399` | Green — positive deltas |

---

## Full Repo Structure After This Push

```
ArcGIS-Hub/
├── home/          ← Homepage (8 files)
├── stats/         ← District Statistics (8 files) ← NEW
├── charts/        ← Old district charts (can retire)
├── districts/     ← Old district cards (can retire)
├── conditions/    ← Housing Conditions (7 files)
├── build/         ← Block the Cuts / Who Owns LB (13 files)
└── README.md
```

Note: The old `charts/` and `districts/` folders from the original light-themed design can be retired once you've verified the new `stats/` folder works correctly.
