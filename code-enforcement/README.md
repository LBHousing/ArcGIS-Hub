# Code Enforcement page — Hub Layout Guide

Replace `BASEURL` with: `https://lbhousing.github.io/ArcGIS-Hub`
All Hub section backgrounds: `#0a0e1a`

The centerpiece is the interactive dashboard (`index.html`) embedded as ONE iframe — its filters
cross-link the map, owner leaderboard, and charts, so it must stay whole. The `?embed=1` flag hides the
dashboard's own title block (the hero below carries it) while keeping its live stat band.

Each iframe needs a **Mobile** and a **Desktop** height (the Hub stores them separately).

---

## Row-by-Row Assembly

### ROW 1 — Hero (iframe)
```
URL:    BASEURL/code-enforcement/hero.html
Height: Mobile 680 · Desktop 580
```

### ROW 2 — Section header "The Map" (text card)
```html
<div style="padding:40px 0 10px;">
  <span style="display:inline-block;font-size:11px;font-weight:600;text-transform:uppercase;letter-spacing:1.5px;padding:5px 14px;border-radius:6px;background:rgba(232,99,109,.1);color:#e8636d;border:1px solid rgba(232,99,109,.2);margin-bottom:12px;">The Map</span>
  <h2 style="font-family:'Segoe UI',system-ui,sans-serif;font-size:36px;font-weight:700;color:#f1f5f9;margin:0 0 6px;">Explore 18 years of violations.</h2>
  <p style="font-family:'Segoe UI',system-ui,sans-serif;font-size:16px;color:#94a3b8;margin:0;font-weight:300;">Filter by year, owner type, district, and violation category. Confirmed violations show by default — toggle in the no-violation complaints to see all enforcement activity.</p>
</div>
```

### ROW 3 — Interactive dashboard (iframe)
```
URL:    BASEURL/code-enforcement/?embed=1
Height: Mobile 2920 · Desktop 1620
```
Heatmap + "Owners on the hook" leaderboard + live filters + charts. Scroll-wheel zoom is disabled so the page scrolls over the map; zoom with the +/- buttons or pinch.

### ROW 4 — Divider (text card)
```html
<div style="height:1px;background:linear-gradient(90deg,transparent,rgba(255,255,255,.06),transparent);"></div>
```

### ROW 5 — Section header "Analysis" (text card)
```html
<div style="padding:40px 0 10px;">
  <span style="display:inline-block;font-size:11px;font-weight:600;text-transform:uppercase;letter-spacing:1.5px;padding:5px 14px;border-radius:6px;background:rgba(52,211,153,.08);color:#34d399;border:1px solid rgba(52,211,153,.2);margin-bottom:12px;">Analysis</span>
  <h2 style="font-family:'Segoe UI',system-ui,sans-serif;font-size:36px;font-weight:700;color:#f1f5f9;margin:0 0 6px;">What the data shows.</h2>
</div>
```

### ROW 6 — Narrative (iframe)
```
URL:    BASEURL/code-enforcement/narrative.html
Height: Mobile 1100 · Desktop 860
```

### ROW 7 — Source banner (text card)
```html
<div style="background:#111827;border:1px solid rgba(255,255,255,.06);border-radius:8px;padding:12px 20px;text-align:center;font-family:'Segoe UI',system-ui,sans-serif;">
  <p style="font-size:12px;color:#64748b;margin:0;line-height:1.6;">Data: <strong style="color:#94a3b8">City of Long Beach</strong> code-enforcement records (Infor public portal) · 142,233 service requests, 48,418 confirmed violations · scraped, geocoded &amp; anonymized by <strong style="color:#94a3b8">LiBRE</strong>, 2026 · personal names removed, entity names retained.</p>
</div>
```

---

## Quick Reference

| Row | Type | Content | Mobile H | Desktop H |
|-----|------|---------|----------|-----------|
| 1 | iframe | Hero + 4 stats | 680 | 580 |
| 2 | text card | "The Map" header | — | — |
| 3 | iframe | **Interactive dashboard** (`?embed=1`) | 2920 | 1620 |
| 4 | text card | Divider | — | — |
| 5 | text card | "Analysis" header | — | — |
| 6 | iframe | Narrative — what the data shows | 1100 | 860 |
| 7 | text card | Source banner | — | — |

**Total: 3 GitHub iframes + 4 Hub text cards.**

---

## GitHub Push Command
```bash
git add code-enforcement/
git commit -m "Code Enforcement Hub page: hero, dashboard embed, narrative"
git push origin main
```
