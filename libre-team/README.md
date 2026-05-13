# Our Team Page — Hub Layout Guide

Replace `BASEURL` with: `https://lbhousing.github.io/ArcGIS-Hub`

All Hub section backgrounds: `#0a0e1a`

---

## Row-by-Row Assembly

### ROW 1 — Hero (GitHub iframe)
```
URL:    BASEURL/team/hero.html
Height: 700
```

### ROW 2 — Marquee (GitHub iframe)
```
URL:    BASEURL/team/marquee.html
Height: 50
```

### ROW 3 — Section header (Hub text card)
```html
<div style="padding:40px 0 10px;">
  <span style="display:inline-block;font-size:16px;font-weight:700;text-transform:uppercase;letter-spacing:2px;padding:10px 28px;border-radius:8px;background:rgba(39,106,219,.12);color:#4d8ae8;border:1px solid rgba(39,106,219,.2);margin-bottom:16px;">Our Partnership</span>
  <h2 style="font-family:'Segoe UI',system-ui,sans-serif;font-size:36px;font-weight:700;color:#f1f5f9;margin:0 0 6px;">Data meets organizing.</h2>
  <p style="font-family:'Segoe UI',system-ui,sans-serif;font-size:16px;color:#94a3b8;margin:0;font-weight:300;">How LiBRE and Cal State Long Beach built a housing data platform together.</p>
</div>
```

### ROW 4 — CSULB collaboration narrative (GitHub iframe)
```
URL:    BASEURL/team/collab.html
Height: 280
```

### ROW 5 — Divider (Hub text card)
```html
<div style="height:1px;background:linear-gradient(90deg,transparent,rgba(255,255,255,.06),transparent);"></div>
```

### ROW 6 — Section header (Hub text card)
```html
<div style="padding:40px 0 10px;">
  <span style="display:inline-block;font-size:16px;font-weight:700;text-transform:uppercase;letter-spacing:2px;padding:10px 28px;border-radius:8px;background:rgba(247,186,33,.1);color:#F7BA21;border:1px solid rgba(247,186,33,.2);margin-bottom:16px;">Partner Organizations</span>
  <h2 style="font-family:'Segoe UI',system-ui,sans-serif;font-size:36px;font-weight:700;color:#f1f5f9;margin:0 0 6px;">Building together.</h2>
</div>
```

### ROW 7 — Partner org cards (GitHub iframe)
```
URL:    BASEURL/team/partners.html
Height: 260
```

### ROW 8 — Divider (Hub text card)

### ROW 9 — Section header (Hub text card)
```html
<div style="padding:40px 0 10px;">
  <span style="display:inline-block;font-size:16px;font-weight:700;text-transform:uppercase;letter-spacing:2px;padding:10px 28px;border-radius:8px;background:rgba(123,78,175,.1);color:#7B4EAF;border:1px solid rgba(123,78,175,.2);margin-bottom:16px;">Leadership</span>
  <h2 style="font-family:'Segoe UI',system-ui,sans-serif;font-size:36px;font-weight:700;color:#f1f5f9;margin:0 0 6px;">Meet the team.</h2>
  <p style="font-family:'Segoe UI',system-ui,sans-serif;font-size:16px;color:#94a3b8;margin:0;font-weight:300;">Together we are tenants, organizers, analysts, and neighbors.</p>
</div>
```

### ROW 10 — Team cards (GitHub iframe)
```
URL:    BASEURL/team/team-cards.html
Height: 280
```

### ROW 11 — Divider (Hub text card)

### ROW 12 — Coming soon bar + note (GitHub iframe)
```
URL:    BASEURL/team/coming-soon-bar.html
Height: 180
```

---

## Quick Reference

| Row | Type | Content | Height |
|-----|------|---------|--------|
| 1 | iframe | Hero | 700 |
| 2 | iframe | Marquee | 50 |
| 3 | text card | "Our Partnership" | — |
| 4 | iframe | CSULB collab narrative | 280 |
| 5 | text card | Divider | — |
| 6 | text card | "Partner Organizations" | — |
| 7 | iframe | LiBRE + CLT cards | 260 |
| 8 | text card | Divider | — |
| 9 | text card | "Leadership" | — |
| 10 | iframe | 3 team cards | 280 |
| 11 | text card | Divider | — |
| 12 | iframe | Coming soon bar + links | 180 |

**Total: 6 GitHub iframes + 6 Hub text cards**

---

## GitHub Push Command

```bash
git add team/
git commit -m "Our Team: modular blocks with CSULB collab, partners, team cards"
git push origin main
```
