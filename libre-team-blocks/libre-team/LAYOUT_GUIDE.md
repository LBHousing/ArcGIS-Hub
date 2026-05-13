# Our Team Page — Hub Layout Guide

Replace `BASEURL` with: `https://lbhousing.github.io/ArcGIS-Hub`

All Hub section backgrounds: `#0a0e1a`

---

## Row-by-Row Assembly (Coming Soon Version)

### ROW 1 — Team Coming Soon (GitHub iframe)
```
URL:    BASEURL/team/coming-soon.html
Height: 1200
```
Full-height page with hero, CSULB collaboration narrative, partner org cards, team preview cards, and coming soon indicator. Single iframe — no additional Hub text cards needed for this version.

---

## Quick Reference

| Row | Type | Content | Height |
|-----|------|---------|--------|
| 1 | iframe | Team coming soon (full page) | 1200 |

**Total: 1 GitHub iframe**

---

## GitHub Push Command

```bash
git add team/
git commit -m "Our Team: coming soon page with CSULB collaboration narrative"
git push origin main
```

---

## Full Repo Structure After This Push

```
ArcGIS-Hub/
├── home/          ← Homepage (8 files)
├── stats/         ← District Statistics (10 files)
├── conditions/    ← Housing Conditions (7 files)
├── build/         ← Block the Cuts (13 files)
├── evictions/     ← Eviction Analysis (8 files)
├── team/          ← Our Team (1 file) ← NEW
└── README.md
```

---

## Future Full Team Page (when ready)

When you have photos, bios, and CSULB student info, the full page will expand to:

| File | Content | Height |
|------|---------|--------|
| `hero.html` | "The people behind the movement" + org stats | 700 |
| `marquee.html` | Scrolling team/impact stats | 50 |
| `staff.html` | Staff photo cards grid | 600 |
| `csulb.html` | CSULB collaboration + student contributors | 500 |
| `partners.html` | Partner org cards | 300 |
| `narr-about.html` | About the collaboration narrative | 400 |

Replace `coming-soon.html` with these modular blocks when ready.
