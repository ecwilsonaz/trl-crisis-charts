# Source Documents

Primary source files for [TRL Crisis Report](https://ecwilsonaz.github.io/trl-crisis-charts/) Parts 1 and 2. Every claim in the report is derived from these public records. Archived March 2026.

## TRL Final Budget Documents

Location: [`trl-budgets/`](./trl-budgets/)

These are the primary source for nearly every number in both parts: salary data, FTE counts, fund balances, revenue, expenditures, and levy rates. Each biennial budget includes audited actuals for 2-3 prior years, allowing cross-referencing across documents.

| File | Originally from | Key data |
|------|----------------|----------|
| `2019-Final-Budget.pdf` | trl.org | 2016-2017 actuals, 2018 estimate, 2019 budget. Department expenditure tables, Position Inventory. |
| `2021-Final-Budget.pdf` | trl.org | 2017-2019 actuals, 2020 estimate, 2021 budget. ED budget message referencing hiring freeze. |
| `2023-Final-Budget.pdf` | trl.org | 2019-2021 actuals, 2022 estimate, 2023 budget. Courier department dissolved into Facilities. |
| `2025-Final-Budget.pdf` | trl.org | 2021-2023 actuals, 2024 estimate, 2025 budget. Levy rate: $0.234024 (p.10). |
| `2026-Final-Budget.pdf` | [trl.org](https://trl.org/wp-content/uploads/sites/140/2025/12/2026-Final-Budget.pdf) | 2022-2024 actuals, 2025 estimate, 2026 budget. Levy rate: $0.228924 (p.9). Position Inventory with admin salary increases (pp.18-22). |

### How salary data was cross-referenced (Exhibit I)

For each year 2017-2024, the "Actual" column from the earliest subsequent budget document was used. Example: the 2021 salary actual comes from the 2023 Final Budget (which labels it "2021 Actual"), not from the 2021 Final Budget (which only has the 2021 adopted budget). Only 2025 (year-end estimate) and 2026 (adopted budget) are non-actual figures.

The six Service Center departments tracked are: Administration, Finance, Human Resources, Information Technology, Creative Services, and Facilities+Courier. These are the departments excluded from AFSCME bargaining unit coverage (except Courier staff, who are represented).

## Washington State Data

Location: [`state-data/`](./state-data/)

| File | Source | Key data |
|------|--------|----------|
| `Merged_WPLSR_data_2024.xlsx` | [Bellingham Public Library](https://bellinghampubliclibrary.org/wplsr-merged) | Washington Public Library Statistical Report, merged 2002-2024. Salary/FTE, expenditures, circulation, population for all WA library systems. Updated March 24, 2026. |
| `2009_Election_Results_All_Counties.xlsx` | WA Secretary of State | County-by-county results for TRL's 2009 levy lid lift attempt. Mason 55.4% yes, Pacific 51.8%, Thurston 46.5%, Grays Harbor 44.3%, Lewis 29.2%. District-wide: 45.1% (failed). |

### How peer comparison was computed (Exhibit J)

Salary per FTE = Total Salary Expenditures / Total FTE for each system and year, from the WPLSR merged dataset. The seven comparison systems: TRL, Fort Vancouver Regional, Kitsap Regional, Pierce County, Sno-Isle, Whatcom County, King County (KCLS, included for scale reference).

## BLS CPI Data

Location: [`bls/`](./bls/)

| File | Source | Key data |
|------|--------|----------|
| `seattle-cpi-u-CUUSA423SA0.csv` | [BLS](https://data.bls.gov/timeseries/CUUSA423SA0) | Seattle-Tacoma-Bellevue CPI-U, semiannual averages. Used for the CPI-adjusted baseline in Exhibit I. 2026 estimated at 3.5% YoY. |

### How the CPI baseline was computed (Exhibit I)

The 2017 Service Center salary total ($2,170,828) is grown at the annual CPI-U rate for each subsequent year: `baseline[year] = baseline[year-1] * (1 + annual_cpi_change)`. The gap between actual spending and this CPI-adjusted baseline is the annual difference shown in the trajectory chart.

## Expense Reports

Location: [`expense-reports/`](./expense-reports/)

| File | Source | Key data |
|------|--------|----------|
| `2026-01-expense-approval-report.pdf` | TRL Board of Trustees February 25, 2026 meeting packet | Line-item expenditures for January 2026. Referenced in Exhibit L audit rationale. |

## Recordings

Board meeting recordings are public records available from TRL. Timestamps in the report reference specific moments in these recordings. Full recordings are too large for GitHub hosting; trimmed clips of key moments may be added in a future update.

All quotes were verified against the original recordings by a human reviewer. Timestamps in the report reference specific moments for independent verification.

## What is NOT included here

- **News articles.** Copyrighted content from Chinook Observer, The Daily Chronicle, HeraldNet, Lynnwood Times, etc. is linked, not rehosted.
- **The anonymous salary spreadsheet.** The report's analysis is built entirely on publicly available TRL Final Budget documents. An anonymously sourced salary spreadsheet was used for early exploration but every number in the published report is independently verifiable from the budget PDFs above.
- **Full meeting recordings.** Too large for GitHub. Available from TRL as public records.

## Version

Sources archived March 2026. The Bellingham WPLSR dataset, BLS CPI data, and TRL budget documents may be updated in future years; the versions hosted here are the ones used in this report.
