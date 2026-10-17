# Amesbury Council On Aging Van Operations Dashboards

Live dashboard: https://djellison.github.io/acoa-van/

A public, no-login view of the ACOA van program's ridership and cashflow, grouped by fiscal quarter (July–June year).

## Contents

- `index.html` – the dashboard page (charts drawn in the browser with d3).
- `data/van_signups.csv` – riders signed up per trip date, Needs vs Social (from the COA Van Signup Macro sheet).
- `data/van_trips.csv` – one row per trip-log entry for both vans (M1443B and M9423B): van, destination, riders, miles, fares, tolls, parking, supplies, gas-card fuel and cash turned in (from the ACOA Van Trip Log). Driver notes are omitted.

## Definitions

- **Needs** – the ONT runs (Our Neighbors' Table plus essentials shopping), mostly Fridays. **Social** – all other outings and events.
- **Net cashflow** – fares minus tolls, parking, supplies and gas-card fuel. Cash turned in to COA staff is a transfer, not a cost.

## Updating

Replace the two CSV files in `data/` with new exports (same columns). The page recalculates everything from them on load.
