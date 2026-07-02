# Australia's Net Zero Progress 🌏

**An interactive data visualisation exploring whether Australia is on track to hit net zero emissions by 2050.**

🔗 **[Live site](https://22kahz.github.io/FIT3179-Visualisation-2/)** | 📂 Built for Monash University FIT3179 (Data Visualisation), Assignment 2

![Vega-Lite](https://img.shields.io/badge/Vega--Lite-Data%20Viz-orange)
![HTML](https://img.shields.io/badge/HTML-81%25-e34c26)
![CSS](https://img.shields.io/badge/CSS-13%25-264de4)
![JavaScript](https://img.shields.io/badge/JavaScript-6%25-f7df1e)

---

## 📖 Overview

Australia signed the Paris Agreement in 2015 and has committed to cutting emissions by 43% (on 2005 levels) by 2030, 62–70% by 2035, and reaching net zero by 2050. This project brings together emissions, energy, and temperature data into a single narrative-driven scrollytelling page to answer one question: **is Australia actually on track?**

The visualisation walks through six chapters:

1. **Global context** — where Australia ranks among the world's per-capita and total CO₂ emitters
2. **Progress tracking** — Australia's emissions trend since 2005 against its 2030/2035 targets
3. **Greenhouse gas breakdown** — CO₂ vs. methane, nitrous oxide, and other gases over time
4. **Sector contribution** — which sectors (electricity, transport, stationary energy, land use) drive emissions
5. **Electricity generation mix** — the shift from coal toward wind and solar
6. **Temperature anomalies** — connecting emissions trends to observed warming

**Key finding:** Australia has cut emissions by ~27–29% since 2005, driven mainly by renewables displacing coal — but progress has flattened since 2020, and non-CO₂ gases plus transport emissions are offsetting gains made in electricity.

## 🧰 Technical Details

| Layer | Technology |
|---|---|
| **Visualisation grammar** | [Vega-Lite](https://vega.github.io/vega-lite/) — declarative JSON specs for each chart, rendered via **Vega-Embed** |
| **Structure & content** | HTML5 |
| **Styling & layout** | CSS3 (custom stylesheet for a scrollytelling, narrative report layout) |
| **Interactivity** | JavaScript — embedding Vega-Lite specs into the page and handling chart interactions |
| **Chart types** | Choropleth/bubble map (global per-capita emissions), multi-line time series with target markers, stacked area charts (GHG type & sector breakdown), interactive legend filtering, streamgraph/area chart for electricity generation mix, diverging bar chart for temperature anomalies |
| **Data processing** | Data cleaned and transformed (normalisation, aggregation by sector/year) prior to visualisation |
| **Hosting** | GitHub Pages (static site) |

### Design choices
- **Scrollytelling format**: charts are embedded alongside narrative text so each visual supports a specific claim, rather than being presented as a standalone dashboard.
- **Interactive legends**: clicking a legend label (e.g. in the sector breakdown chart) isolates that series, letting the reader explore the data themselves.
- **Consistent target/annotation layers**: reference lines and markers (e.g. 2030/2035 targets) are layered directly onto the relevant charts using Vega-Lite's layering support, rather than relying on prose alone.

## 📊 Data Sources

- [Our World in Data — CO₂ and Greenhouse Gas Emissions](https://ourworldindata.org/co2-and-greenhouse-gas-emissions)
- [Australian Government DCCEEW — Electricity and Energy Sector Plan](https://www.dcceew.gov.au/climate-change/emissions-reduction/net-zero/electricity-and-energy-sector-plan)
- [DCCEEW — National Greenhouse Gas Inventory Quarterly Update](https://www.dcceew.gov.au/climate-change/publications/national-greenhouse-gas-inventory-quarterly-update-march-2025)
- [Open Electricity](https://explore.openelectricity.org.au/energy/au/)

This project was completed as **Assignment 2** for **FIT3179: Data Visualisation** at Monash University, focused on applying visualisation grammar (Vega-Lite) to build maps and charts around a real-world dataset, presented as a public web page with an accompanying analytical report.

---

**Author:** Anzo Adrien Ariandrie
