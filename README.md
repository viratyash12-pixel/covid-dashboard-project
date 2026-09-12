# covid-dashboard-project
## COVID-19 Global Dashboard

A self-contained, interactive HTML dashboard for visualizing COVID-19 case, death, and vaccination trends. Built with vanilla JavaScript and Chart.js — no server, build step, or dependencies required. Just open the file in a browser.

### Features

- **8 KPI cards** — Total Cases, Total Deaths, Death Rate, % Population Infected, Total Vaccinations, % Population Vaccinated, Latest Week New Cases (w/ week-over-week change), Countries Tracked
- **4 interactive charts** — weekly new-cases trend, case share by continent (doughnut), total deaths by country (bar), % population vaccinated by country (bar)
- **Sortable data table** — per-country snapshot with click-to-sort columns
- **Live filters** — continent, country, and date range, all updating KPIs, charts, and the table simultaneously

### Data

Ships with a realistic sample dataset (10 countries, weekly, Jan–Jun 2021) generated to resemble typical COVID-19 reporting patterns — not actual historical figures. To use real data, replace the `DATA` array in the `<script>` tag with rows shaped like:

​```json
{
  "location": "United States",
  "continent": "North America",
  "date": "2021-01-03",
  "population": 331000000,
  "new_cases": 12000,
  "total_cases": 500000,
  "new_deaths": 300,
  "total_deaths": 15000,
  "new_vaccinations": 0,
  "total_vaccinations": 0
}
​```

### Tech

Pure HTML/CSS/JavaScript + [Chart.js](https://www.chartjs.org/) (via CDN). No build tools, no backend, no API keys.
