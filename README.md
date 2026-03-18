# LiBRE District Statistics — GitHub Pages Charts

Interactive housing cost burden charts for the [LiBRE District Statistics](https://weare-libre.hub.arcgis.com/pages/district-statistics) Hub page.

## Setup

1. Push this repo to GitHub
2. Go to **Settings → Pages → Source → Deploy from branch → main**
3. Wait ~1 minute for GitHub Pages to build
4. Your charts will be live at: `https://YOUR-USERNAME.github.io/REPO-NAME/`

## File Structure

```
├── charts/
│   ├── metrics.html              ← Headline metric cards
│   ├── all-renters-rate.html     ← All renters: burden rate trend
│   ├── all-renters-count.html    ← All renters: household count trend
│   ├── seniors-rate.html         ← 65+ seniors: burden rate trend
│   ├── seniors-count.html        ← 65+ seniors: household count trend
│   ├── lowincome-rate.html       ← Low-income: severe rate trend
│   ├── lowincome-count.html      ← Low-income: displacement count
│   ├── district-bars-all-renters.html  ← District comparison bars
│   ├── district-bars-seniors.html
│   └── district-bars-lowincome.html
├── districts/
│   ├── district-1.html           ← District 1 card with sparklines
│   ├── district-2.html
│   ├── ...
│   └── district-9.html
└── README.md
```

## Hub Iframe Embed Codes

Replace `YOUR-USERNAME` and `REPO-NAME` with your actual GitHub username and repository name.

### Headline Metrics
```html
<iframe src="https://YOUR-USERNAME.github.io/REPO-NAME/charts/metrics.html" 
  width="100%" height="200" frameborder="0" scrolling="no"
  title="Citywide headline statistics"></iframe>
```

### All Renters — Rate Trend
```html
<iframe src="https://YOUR-USERNAME.github.io/REPO-NAME/charts/all-renters-rate.html" 
  width="100%" height="380" frameborder="0" scrolling="no"
  title="All renters cost burden rate trend"></iframe>
```

### All Renters — Count Trend
```html
<iframe src="https://YOUR-USERNAME.github.io/REPO-NAME/charts/all-renters-count.html" 
  width="100%" height="380" frameborder="0" scrolling="no"
  title="All renters household count trend"></iframe>
```

### 65+ Seniors — Rate Trend
```html
<iframe src="https://YOUR-USERNAME.github.io/REPO-NAME/charts/seniors-rate.html" 
  width="100%" height="380" frameborder="0" scrolling="no"
  title="Senior 65+ burden rate trend"></iframe>
```

### 65+ Seniors — Count Trend
```html
<iframe src="https://YOUR-USERNAME.github.io/REPO-NAME/charts/seniors-count.html" 
  width="100%" height="380" frameborder="0" scrolling="no"
  title="Senior 65+ household count trend"></iframe>
```

### Low-Income — Rate Trend
```html
<iframe src="https://YOUR-USERNAME.github.io/REPO-NAME/charts/lowincome-rate.html" 
  width="100%" height="380" frameborder="0" scrolling="no"
  title="Low-income severe burden rate trend"></iframe>
```

### Low-Income — Count Trend (Displacement)
```html
<iframe src="https://YOUR-USERNAME.github.io/REPO-NAME/charts/lowincome-count.html" 
  width="100%" height="380" frameborder="0" scrolling="no"
  title="Low-income household displacement trend"></iframe>
```

### District Comparison — All Renters
```html
<iframe src="https://YOUR-USERNAME.github.io/REPO-NAME/charts/district-bars-all-renters.html" 
  width="100%" height="400" frameborder="0" scrolling="no"
  title="District comparison all renters"></iframe>
```

### District Comparison — Seniors
```html
<iframe src="https://YOUR-USERNAME.github.io/REPO-NAME/charts/district-bars-seniors.html" 
  width="100%" height="400" frameborder="0" scrolling="no"
  title="District comparison seniors"></iframe>
```

### District Comparison — Low-Income
```html
<iframe src="https://YOUR-USERNAME.github.io/REPO-NAME/charts/district-bars-lowincome.html" 
  width="100%" height="400" frameborder="0" scrolling="no"
  title="District comparison low-income"></iframe>
```

### District Cards (1-9)
```html
<iframe src="https://YOUR-USERNAME.github.io/REPO-NAME/districts/district-1.html" 
  width="100%" height="620" frameborder="0" scrolling="no"
  title="District 1 housing statistics"></iframe>
```
```html
<iframe src="https://YOUR-USERNAME.github.io/REPO-NAME/districts/district-2.html" 
  width="100%" height="620" frameborder="0" scrolling="no"
  title="District 2 housing statistics"></iframe>
```
```html
<iframe src="https://YOUR-USERNAME.github.io/REPO-NAME/districts/district-3.html" 
  width="100%" height="620" frameborder="0" scrolling="no"
  title="District 3 housing statistics"></iframe>
```
```html
<iframe src="https://YOUR-USERNAME.github.io/REPO-NAME/districts/district-4.html" 
  width="100%" height="620" frameborder="0" scrolling="no"
  title="District 4 housing statistics"></iframe>
```
```html
<iframe src="https://YOUR-USERNAME.github.io/REPO-NAME/districts/district-5.html" 
  width="100%" height="620" frameborder="0" scrolling="no"
  title="District 5 housing statistics"></iframe>
```
```html
<iframe src="https://YOUR-USERNAME.github.io/REPO-NAME/districts/district-6.html" 
  width="100%" height="620" frameborder="0" scrolling="no"
  title="District 6 housing statistics"></iframe>
```
```html
<iframe src="https://YOUR-USERNAME.github.io/REPO-NAME/districts/district-7.html" 
  width="100%" height="620" frameborder="0" scrolling="no"
  title="District 7 housing statistics"></iframe>
```
```html
<iframe src="https://YOUR-USERNAME.github.io/REPO-NAME/districts/district-8.html" 
  width="100%" height="620" frameborder="0" scrolling="no"
  title="District 8 housing statistics"></iframe>
```
```html
<iframe src="https://YOUR-USERNAME.github.io/REPO-NAME/districts/district-9.html" 
  width="100%" height="620" frameborder="0" scrolling="no"
  title="District 9 housing statistics"></iframe>
```

## Suggested Hub Page Layout

| Row | Left Column | Right Column |
|-----|------------|--------------|
| 1   | **Headline Metrics** (full width) | |
| 2   | *Section header text: "Total Rent Burden Households"* | |
| 3   | All Renters Rate Trend | All Renters Count Trend |
| 4   | *Section header text: "65+ Senior Households"* | |
| 5   | Seniors Rate Trend | Seniors Count Trend |
| 6   | *Section header text: "Low-Income Severe Burden"* | |
| 7   | Low-Income Rate Trend | Low-Income Count Trend |
| 8   | *Section header text: "District Comparison"* | |
| 9   | District Bars Renters | District Bars Seniors |
| 10  | District Bars Low-Income (full width) | |
| 11  | *Narrative text (use Hub text card, no iframe)* | |
| 12  | District 1 | District 2 |
| 13  | District 3 | District 4 |
| 14  | District 5 | District 6 |
| 15  | District 7 | District 8 |
| 16  | District 9 | |

## Updating Yearly

1. Run your Census API Python scripts to get new data
2. Edit the data arrays in each HTML file (search for the array values)
3. Update headline metrics text in `charts/metrics.html`
4. Commit and push — GitHub Pages auto-deploys

## Data Sources

- **B25070**: Gross Rent as % of Household Income (all renters)
- **B25072**: Age of Householder by Gross Rent (65+ seniors)
- **B25074**: Household Income by Gross Rent (low-income <$35K)
- U.S. Census Bureau ACS 5-Year Estimates, 2010-2014 through 2020-2024
- Weighted by census tract area overlap with Long Beach council districts
