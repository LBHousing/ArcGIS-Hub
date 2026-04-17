# Block the Cuts & Build LB — Hub Layout Guide

Replace `BASEURL` with: `https://lbhousing.github.io/ArcGIS-Hub`

All Hub section backgrounds: `#0a0e1a`

---

## Row-by-Row Assembly

### ROW 1 — Hero (GitHub iframe)
```
URL:    BASEURL/build/hero.html
Height: 700
```

### ROW 2 — Marquee (GitHub iframe)
```
URL:    BASEURL/build/marquee.html
Height: 50
```

### ROW 3 — Section header "Citywide Ownership" (Hub text card)
```html
<div style="padding:40px 0 10px;">
  <div style="font-family:'Segoe UI',system-ui,sans-serif;font-size:80px;font-weight:300;color:#252d4a;line-height:1;">01</div>
  <span style="display:inline-block;font-size:11px;font-weight:600;text-transform:uppercase;letter-spacing:1.5px;padding:5px 14px;border-radius:6px;background:rgba(39,106,219,.12);color:#4d8ae8;border:1px solid rgba(39,106,219,.2);margin-bottom:12px;">Citywide Ownership</span>
  <h2 style="font-family:'Segoe UI',system-ui,sans-serif;font-size:36px;font-weight:700;color:#f1f5f9;margin:0 0 6px;">Every parcel. Every owner type. The full picture.</h2>
  <p style="font-family:'Segoe UI',system-ui,sans-serif;font-size:16px;color:#94a3b8;margin:0;font-weight:300;">All 186,658 dwelling units in Long Beach, broken down by who holds title — and how each category's share is shifting.</p>
</div>
```

### ROW 4 — Metric bars (GitHub iframe)
```
URL:    BASEURL/build/metric-bars.html
Height: 260
```

### ROW 5 — Ownership charts: donut + YOY (GitHub iframe)
```
URL:    BASEURL/build/charts-ownership.html
Height: 400
```

### ROW 6 — Divider (Hub text card)
```html
<div style="height:1px;background:linear-gradient(90deg,transparent,rgba(255,255,255,.06),transparent);"></div>
```

### ROW 7 — Section header "The Ownership Shift" (Hub text card)
```html
<div style="padding:40px 0 10px;">
  <div style="font-family:'Segoe UI',system-ui,sans-serif;font-size:80px;font-weight:300;color:#252d4a;line-height:1;">02</div>
  <span style="display:inline-block;font-size:11px;font-weight:600;text-transform:uppercase;letter-spacing:1.5px;padding:5px 14px;border-radius:6px;background:rgba(210,51,63,.1);color:#D2333F;border:1px solid rgba(210,51,63,.2);margin-bottom:12px;">The Ownership Shift</span>
  <h2 style="font-family:'Segoe UI',system-ui,sans-serif;font-size:36px;font-weight:700;color:#f1f5f9;margin:0 0 6px;">Individuals out. Entities in. 2,867 units lost.</h2>
  <p style="font-family:'Segoe UI',system-ui,sans-serif;font-size:16px;color:#94a3b8;margin:0;font-weight:300;">Housing is moving from individual homeowners to LLCs, corporations, and partnerships.</p>
</div>
```

### ROW 8 — Owner type charts: parcels + units (GitHub iframe)
```
URL:    BASEURL/build/charts-owner-type.html
Height: 400
```

### ROW 9 — Shift narrative (GitHub iframe)
```
URL:    BASEURL/build/narr-shift.html
Height: 320
```

### ROW 10 — Divider (Hub text card)

### ROW 11 — Section header "The Trust Loophole" (Hub text card)
```html
<div style="padding:40px 0 10px;">
  <div style="font-family:'Segoe UI',system-ui,sans-serif;font-size:80px;font-weight:300;color:#252d4a;line-height:1;">03</div>
  <span style="display:inline-block;font-size:11px;font-weight:600;text-transform:uppercase;letter-spacing:1.5px;padding:5px 14px;border-radius:6px;background:rgba(247,186,33,.1);color:#F7BA21;border:1px solid rgba(247,186,33,.2);margin-bottom:12px;">The Trust Loophole</span>
  <h2 style="font-family:'Segoe UI',system-ui,sans-serif;font-size:36px;font-weight:700;color:#f1f5f9;margin:0 0 6px;">3,451 trusts own multiple properties. 194 average 25 units each.</h2>
  <p style="font-family:'Segoe UI',system-ui,sans-serif;font-size:16px;color:#94a3b8;margin:0;font-weight:300;">Individual trusts get homeowner exemptions — but many operate at institutional scale.</p>
</div>
```

### ROW 12 — Trust metric bars (GitHub iframe)
```
URL:    BASEURL/build/metric-trusts.html
Height: 180
```

### ROW 13 — Trust narrative (GitHub iframe)
```
URL:    BASEURL/build/narr-trusts.html
Height: 340
```

### ROW 14 — Divider (Hub text card)

### ROW 15 — Section header "Ownership Concentration" (Hub text card)
```html
<div style="padding:40px 0 10px;">
  <div style="font-family:'Segoe UI',system-ui,sans-serif;font-size:80px;font-weight:300;color:#252d4a;line-height:1;">04</div>
  <span style="display:inline-block;font-size:11px;font-weight:600;text-transform:uppercase;letter-spacing:1.5px;padding:5px 14px;border-radius:6px;background:rgba(210,51,63,.1);color:#D2333F;border:1px solid rgba(210,51,63,.2);margin-bottom:12px;">Ownership Concentration</span>
  <h2 style="font-family:'Segoe UI',system-ui,sans-serif;font-size:36px;font-weight:700;color:#f1f5f9;margin:0 0 6px;">A small number of owners control a large share of the city.</h2>
  <p style="font-family:'Segoe UI',system-ui,sans-serif;font-size:16px;color:#94a3b8;margin:0;font-weight:300;">4,548 multi-property owners control 38,945 units — 34.8% of the city's estimated rental stock.</p>
</div>
```

### ROW 16 — Concentration chart (GitHub iframe)
```
URL:    BASEURL/build/chart-concentration.html
Height: 400
```

### ROW 17 — Divider (Hub text card)

### ROW 18 — Section header "Largest Owners" (Hub text card)
```html
<div style="padding:40px 0 10px;">
  <div style="font-family:'Segoe UI',system-ui,sans-serif;font-size:80px;font-weight:300;color:#252d4a;line-height:1;">05</div>
  <span style="display:inline-block;font-size:11px;font-weight:600;text-transform:uppercase;letter-spacing:1.5px;padding:5px 14px;border-radius:6px;background:rgba(247,186,33,.1);color:#F7BA21;border:1px solid rgba(247,186,33,.2);margin-bottom:12px;">Largest Owners</span>
  <h2 style="font-family:'Segoe UI',system-ui,sans-serif;font-size:36px;font-weight:700;color:#f1f5f9;margin:0 0 6px;">The 25 biggest entity owners in Long Beach.</h2>
  <p style="font-family:'Segoe UI',system-ui,sans-serif;font-size:16px;color:#94a3b8;margin:0;font-weight:300;">The top owner controls 538 units on just 2 parcels.</p>
</div>
```

### ROW 19 — Top 25 chart (GitHub iframe)
```
URL:    BASEURL/build/chart-top25.html
Height: 780
```

### ROW 20 — Divider (Hub text card)

### ROW 21 — Section header "Renter Protections" (Hub text card)
```html
<div style="padding:40px 0 10px;">
  <div style="font-family:'Segoe UI',system-ui,sans-serif;font-size:80px;font-weight:300;color:#252d4a;line-height:1;">06</div>
  <span style="display:inline-block;font-size:11px;font-weight:600;text-transform:uppercase;letter-spacing:1.5px;padding:5px 14px;border-radius:6px;background:rgba(52,211,153,.08);color:#34d399;border:1px solid rgba(52,211,153,.2);margin-bottom:12px;">Renter Protections</span>
  <h2 style="font-family:'Segoe UI',system-ui,sans-serif;font-size:36px;font-weight:700;color:#f1f5f9;margin:0 0 6px;">What this means for tenant protections.</h2>
</div>
```

### ROW 22 — Protections narrative (GitHub iframe)
```
URL:    BASEURL/build/narr-protections.html
Height: 620
```

### ROW 23 — Divider (Hub text card)

### ROW 24 — Section header "Historical Context" (Hub text card)
```html
<div style="padding:40px 0 10px;">
  <div style="font-family:'Segoe UI',system-ui,sans-serif;font-size:80px;font-weight:300;color:#252d4a;line-height:1;">07</div>
  <span style="display:inline-block;font-size:11px;font-weight:600;text-transform:uppercase;letter-spacing:1.5px;padding:5px 14px;border-radius:6px;background:rgba(39,106,219,.12);color:#4d8ae8;border:1px solid rgba(39,106,219,.2);margin-bottom:12px;">Historical Context</span>
  <h2 style="font-family:'Segoe UI',system-ui,sans-serif;font-size:36px;font-weight:700;color:#f1f5f9;margin:0 0 6px;">15 years of growth. $59.5 billion in assessed value.</h2>
</div>
```

### ROW 25 — Historical charts (GitHub iframe)
```
URL:    BASEURL/build/charts-historical.html
Height: 400
```

### ROW 26 — Know your rights (GitHub iframe)
```
URL:    BASEURL/build/know-your-rights.html
Height: 340
```

---

## Quick Reference

| Row | Type | Content | Height |
|-----|------|---------|--------|
| 1 | iframe | Hero + counters | 700 |
| 2 | iframe | Marquee | 50 |
| 3 | text card | "01 Citywide Ownership" | — |
| 4 | iframe | Metric bars (6) | 260 |
| 5 | iframe | Donut + YOY charts | 400 |
| 6 | text card | Divider | — |
| 7 | text card | "02 The Ownership Shift" | — |
| 8 | iframe | Owner type bars (2) | 400 |
| 9 | iframe | Shift narrative | 320 |
| 10 | text card | Divider | — |
| 11 | text card | "03 The Trust Loophole" | — |
| 12 | iframe | Trust metric bars (3) | 180 |
| 13 | iframe | Trust narrative | 340 |
| 14 | text card | Divider | — |
| 15 | text card | "04 Concentration" | — |
| 16 | iframe | Concentration chart | 400 |
| 17 | text card | Divider | — |
| 18 | text card | "05 Largest Owners" | — |
| 19 | iframe | Top 25 horizontal bar | 780 |
| 20 | text card | Divider | — |
| 21 | text card | "06 Renter Protections" | — |
| 22 | iframe | Protections narrative | 620 |
| 23 | text card | Divider | — |
| 24 | text card | "07 Historical Context" | — |
| 25 | iframe | Historical charts (2) | 400 |
| 26 | iframe | Know Your Rights | 340 |

**Total: 13 GitHub iframes + 13 Hub text cards**

---

## GitHub Push Command

```bash
git add build/
git commit -m "Block the Cuts page: hero, marquee, metrics, charts, narratives, top 25, rights"
git push origin main
```

---

## Full Repo Structure After This Push

```
ArcGIS-Hub/
├── home/          ← Homepage (8 files)
├── charts/        ← District Statistics charts (12+ files)
├── districts/     ← District cards D1-D9 (9 files)
├── conditions/    ← Housing Conditions (7 files)
├── build/         ← Block the Cuts / Who Owns LB (13 files)
└── README.md
```
