# US Car Cost Data by State (2026)

Free, open datasets on what it costs to buy, register and charge a car in every US state and DC, compiled and maintained by **[CarCostWise](https://carcostwise.com/)**.

Each file is a plain CSV covering all 50 states and DC, built from official state agencies and named public sources (listed in [SOURCES.md](SOURCES.md)). Use them in articles, research, calculators or classroom work.

## Datasets

| File | What it covers | Full write-up |
|---|---|---|
| [`car-sales-tax-by-state-2026.csv`](car-sales-tax-by-state-2026.csv) | State sales tax on vehicle purchases, whether local tax is added, trade-in credit rules, notes | [Car sales tax by state (2026)](https://carcostwise.com/buying/car-sales-tax-by-state/) |
| [`ev-registration-fees-by-state-2026.csv`](ev-registration-fees-by-state-2026.csv) | Extra annual registration fees for EVs, plug-in hybrids and hybrids, with effective dates | [EV registration fees by state (2026)](https://carcostwise.com/ownership/ev-registration-fees-by-state/) |
| [`ev-home-charging-cost-by-state-2026.csv`](ev-home-charging-cost-by-state-2026.csv) | Residential electricity price (Aug 2026, cents/kWh), cost of a full 75 kWh charge, cost per 1,000 miles, plus the US average | [Cost to charge an EV at home by state (2026)](https://carcostwise.com/fuel/cost-to-charge-electric-car-at-home-by-state/) |

## Quick start

```python
import pandas as pd
tax = pd.read_csv("https://raw.githubusercontent.com/raselhk/car-cost-data/main/car-sales-tax-by-state-2026.csv")
print(tax.head())
```

## Updates

- Sales tax and EV fees: reviewed when state laws change (EV fees are next reviewed in December 2026).
- Home charging: refreshed with each new monthly EIA electricity price release.

Found an error or a newer rate? Open an issue with the state and a source link.

## License and attribution

The data is released under [CC BY 4.0](LICENSE). You may copy, share and adapt it, including commercially, as long as you credit the source:

> Source: [CarCostWise](https://carcostwise.com/), US Car Cost Data by State (2026)

Figures are for information only. Rates change, so check with your state DMV or revenue department before you buy or register a vehicle.
