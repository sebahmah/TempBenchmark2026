# TempBenchmark2026

Temperature benchmark for five foodcourts (Palas, IMTM, IMSV, IMCJ, IMIS), 1 Jun – 30 Sep 2026, built from 30-minute BMS sensor readings (23 sensors).

Open `index.html` in a browser, or view it through GitHub Pages.

## What it shows
- Monthly and period average temperature per sensor, per foodcourt and for the portfolio
- Each foodcourt vs the portfolio average (°C difference)
- Daily group P10 / P50 / P90 across all sensors
- Per foodcourt and month, % of days whose daily average sits inside the group P10–P90 band

## Method
- **Foodcourt average:** mean of its sensors at each reading, then averaged over the period. Missing readings are skipped.
- **Portfolio average:** simple mean of the five foodcourt averages (equal weight).
- **Group percentiles:** per day, over every reading from all sensors in all foodcourts.
- **In band:** foodcourt daily average between that day's group P10 and P90, inclusive.

## Data
`data/` holds the aggregated CSVs the page uses. Raw half-hourly exports are not included.
