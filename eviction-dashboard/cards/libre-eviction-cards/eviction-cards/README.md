# Long Beach eviction cards

Each file here is a self contained single card. It carries its own data, styling, and
libraries, so you can embed any one of them on its own in the ArcGIS Hub using an Iframe
card. None of these depend on the interactive filters from the main dashboard, so they
render the same everywhere.

Host them alongside the main dashboard, for example at
`https://lbhousing.github.io/ArcGIS-Hub/eviction-cards/trend.html`, then paste that URL
into a Hub Iframe card.

## The cards

| File | What it shows | Suggested iframe height |
| --- | --- | --- |
| `headline-numbers.html` | Five big numbers: total actions, households, notices, lockouts, lockout rate | 500 |
| `trend.html` | Notices versus lockouts by year, with the policy markers | 540 |
| `policy-impact.html` | The written story of what the timeline shows | 440 |
| `cohort.html` | Eventual lockout rate by notice cohort | 520 |
| `seasonality.html` | Notices by calendar month across all years | 500 |
| `funnel.html` | The path from notice to lockout, all years | 320 |
| `owner-type.html` | Notices and lockouts by owner type | 580 |
| `top-filers.html` | Table of the largest filers | 660 |
| `data-quality.html` | What was wrong with the old numbers | 400 |

## Notes on height

The heights above suit a normal desktop width. The two text cards, `policy-impact.html`
and `data-quality.html`, reflow into a single column on narrow phone screens and grow
taller there. For those two, either raise the height or set the Hub Iframe scrolling
option to Auto so the reader can scroll inside the card.

## Data

Every card uses only aggregate figures. There are no individual addresses, no map points,
and no tenant names. Individual owner names in the filers table are masked as IND_number.
The numbers come from Los Angeles County Superior Court records rebuilt from source. The
year 2016 was not released by the county, so it is absent everywhere.
