# Our Team Page — Hub Layout Guide (v3)

Replace `BASEURL` with: `https://lbhousing.github.io/ArcGIS-Hub`

All Hub section backgrounds: `#0a0e1a`

This v3 reflects the final structure: Dr. Gary Hytrek folded into the team cards (no separate Board of Directors section), Block the Cuts campaign linked, DSLC simplified to a single deck link, and the active-collaborations TBD slot removed.

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
Height: 60
```

### ROW 3 — Section header (Hub text card)
```html
<div style="padding:40px 0 10px;">
  <span style="display:inline-block;font-size:16px;font-weight:700;text-transform:uppercase;letter-spacing:2px;padding:10px 28px;border-radius:8px;background:rgba(39,106,219,.12);color:#4d8ae8;border:1px solid rgba(39,106,219,.2);margin-bottom:16px;">Our Origins</span>
  <h2 style="font-family:'Segoe UI',system-ui,sans-serif;font-size:36px;font-weight:700;color:#f1f5f9;margin:0 0 6px;">From thesis to public platform.</h2>
  <p style="font-family:'Segoe UI',system-ui,sans-serif;font-size:16px;color:#94a3b8;margin:0;font-weight:300;">A 2019 graduate research project, continued and expanded into the LiBRE data platform.</p>
</div>
```

### ROW 4 — Origins narrative (GitHub iframe)
```
URL:    BASEURL/team/origins.html
Height: 500
```

### ROW 5 — Divider (Hub text card)
```html
<div style="height:1px;background:linear-gradient(90deg,transparent,rgba(255,255,255,.06),transparent);"></div>
```

### ROW 6 — Section header (Hub text card)
```html
<div style="padding:40px 0 10px;">
  <span style="display:inline-block;font-size:16px;font-weight:700;text-transform:uppercase;letter-spacing:2px;padding:10px 28px;border-radius:8px;background:rgba(247,186,33,.1);color:#F7BA21;border:1px solid rgba(247,186,33,.2);margin-bottom:16px;">Our Partners</span>
  <h2 style="font-family:'Segoe UI',system-ui,sans-serif;font-size:36px;font-weight:700;color:#f1f5f9;margin:0 0 6px;">Building together.</h2>
  <p style="font-family:'Segoe UI',system-ui,sans-serif;font-size:16px;color:#94a3b8;margin:0;font-weight:300;">Funders, coalition partners, and the academic network behind the project.</p>
</div>
```

### ROW 7 — Partner organizations (GitHub iframe)
```
URL:    BASEURL/team/partners.html
Height: 560
```

### ROW 8 — Divider (Hub text card)

### ROW 9 — Section header (Hub text card)
```html
<div style="padding:40px 0 10px;">
  <span style="display:inline-block;font-size:16px;font-weight:700;text-transform:uppercase;letter-spacing:2px;padding:10px 28px;border-radius:8px;background:rgba(123,78,175,.1);color:#7B4EAF;border:1px solid rgba(123,78,175,.2);margin-bottom:16px;">Leadership</span>
  <h2 style="font-family:'Segoe UI',system-ui,sans-serif;font-size:36px;font-weight:700;color:#f1f5f9;margin:0 0 6px;">Meet the team.</h2>
  <p style="font-family:'Segoe UI',system-ui,sans-serif;font-size:16px;color:#94a3b8;margin:0;font-weight:300;">LiBRE staff and board carrying the day-to-day and strategic work.</p>
</div>
```

### ROW 10 — Team cards (GitHub iframe)
```
URL:    BASEURL/team/team-cards.html
Height: 360
```

### ROW 11 — Divider (Hub text card)

### ROW 12 — Section header (Hub text card)
```html
<div style="padding:40px 0 10px;">
  <span style="display:inline-block;font-size:16px;font-weight:700;text-transform:uppercase;letter-spacing:2px;padding:10px 28px;border-radius:8px;background:rgba(52,211,153,.08);color:#34d399;border:1px solid rgba(52,211,153,.2);margin-bottom:16px;">Student Research</span>
  <h2 style="font-family:'Segoe UI',system-ui,sans-serif;font-size:36px;font-weight:700;color:#f1f5f9;margin:0 0 6px;">LB&ndash;C Data Science Learning Community.</h2>
  <p style="font-family:'Segoe UI',system-ui,sans-serif;font-size:16px;color:#94a3b8;margin:0;font-weight:300;">Summer 2025 student research projects, faculty-advised through CSULB.</p>
</div>
```

### ROW 13 — DSLC team + research projects (GitHub iframe)
```
URL:    BASEURL/team/dslc.html
Height: 1200
```

### ROW 14 — Divider (Hub text card)

### ROW 15 — Section header (Hub text card)
```html
<div style="padding:40px 0 10px;">
  <span style="display:inline-block;font-size:16px;font-weight:700;text-transform:uppercase;letter-spacing:2px;padding:10px 28px;border-radius:8px;background:rgba(210,51,63,.1);color:#D2333F;border:1px solid rgba(210,51,63,.2);margin-bottom:16px;">Active Collaborations</span>
  <h2 style="font-family:'Segoe UI',system-ui,sans-serif;font-size:36px;font-weight:700;color:#f1f5f9;margin:0 0 6px;">Student contributors &amp; ongoing work.</h2>
  <p style="font-family:'Segoe UI',system-ui,sans-serif;font-size:16px;color:#94a3b8;margin:0;font-weight:300;">Individual contributors building specific projects within the LiBRE platform.</p>
</div>
```

### ROW 16 — Active collaborations cards (GitHub iframe)
```
URL:    BASEURL/team/collabs.html
Height: 360
```

### ROW 17 — Divider (Hub text card)

### ROW 18 — Updates bar (GitHub iframe)
```
URL:    BASEURL/team/updates-bar.html
Height: 220
```

---

## Quick Reference

| Row | Type | Content | Height |
|-----|------|---------|--------|
| 1 | iframe | Hero (Est. 2019) | 700 |
| 2 | iframe | Marquee | 60 |
| 3 | text card | "Our Origins" header | — |
| 4 | iframe | Origins narrative | 500 |
| 5 | text card | Divider | — |
| 6 | text card | "Our Partners" header | — |
| 7 | iframe | 5 partner cards | 560 |
| 8 | text card | Divider | — |
| 9 | text card | "Leadership" header | — |
| 10 | iframe | Team cards (4: Andre, Kevin, Nazir, Dr. Hytrek) | 360 |
| 11 | text card | Divider | — |
| 12 | text card | "Student Research / DSLC" header | — |
| 13 | iframe | DSLC: faculty + 6 students + 4 projects + deck link | 1200 |
| 14 | text card | Divider | — |
| 15 | text card | "Active Collaborations" header | — |
| 16 | iframe | Samuel Flexo + Paul Labelle | 360 |
| 17 | text card | Divider | — |
| 18 | iframe | Updates bar + footer note | 220 |

**Total: 8 GitHub iframes + 10 Hub text cards**

---

## Files in this push

```
team/
├── hero.html              ← Est. 2019, six years in the making
├── marquee.html           ← Refreshed stats
├── origins.html           ← Narrative: 2019 thesis → 2022 Kevin/NALCAB → 2023 launch
├── partners.html          ← LiBRE / NALCAB / LAANE / CSULB Geog / LB-C DSLC
├── team-cards.html        ← LiBRE staff + Dr. Gary Hytrek
├── dslc.html              ← Flyer + Jonathan Ocón + 6 students + 4 research tracks
├── collabs.html           ← Samuel Flexo + Paul Labelle
├── updates-bar.html       ← "More contributors ahead" footer
├── img/
│   └── dslc-flyer.png     ← DSLC research presentations flyer
└── LAYOUT_GUIDE.md        ← This file
```

The old `coming-soon.html` and the no-longer-used `board.html` can be deleted from the repo if they were ever pushed.

---

## Outstanding TBD items (in-file HTML comments)

Each `<!-- TBD: -->` comment in the HTML marks content to refine later:

**`partners.html`**
- NALCAB grant scope: tighten to specific year and program description
- CSULB Geography: tone of relationship (institutional vs. individual-faculty)
- LB-C DSLC: formal governance and host institution

**`collabs.html`**
- Samuel Flexo: tighten environmental dashboard scope
- Paul Labelle / CLT mapping: project specifics, stage, deliverables

---

## GitHub Push Command

```bash
# From repo root after copying files into team/
git add team/
git rm team/coming-soon.html  # if it still exists
git rm team/board.html        # if a previous draft was pushed
git commit -m "Our Team v3: origins, partners, team+board merged, DSLC, contributors"
git push origin main
```

---

## Image asset

`team/img/dslc-flyer.png` is the LB-Compton Data Science Learning Community Research Presentations flyer used in the DSLC section. If you have a higher-resolution version, swap the file in place — no HTML changes needed.

---

## Block the Cuts campaign reference

The LAANE collaboration is now linked to the campaign page at `https://www.wearelbre.org/build-long-beach`. Both `partners.html` (LAANE card body) and `origins.html` (footer note) reference it. Update both files together if the URL ever changes.
