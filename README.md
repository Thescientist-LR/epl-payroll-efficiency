# EPL Payroll Efficiency — Finding the Underdogs

**Premier League 2023/24 · Tioluwani Olubowale · Python, pandas and Tableau**

Did clubs with smaller payrolls win more matches than their budgets suggested? Six of ten clubs below the £75.514m league median beat their payroll-based wins benchmark. Six of ten clubs in the other half did too. Wolves and Bournemouth stood out individually, while the two groups exceeded the benchmark equally often.

| Club | What stood out |
|---|---|
| Wolves | Won 13 matches against a benchmark of 10.62, the largest positive gap among lower-payroll clubs (+2.38). |
| Bournemouth | Won 13 against a benchmark of 10.73 (+2.27). |
| Brentford | Recorded the lowest payroll per win (£3.99m). Its 10 wins exceeded its benchmark by 0.88. |
| Manchester United | Recorded the highest payroll per win (£11.43m). Its 18 wins fell 9.01 short of its benchmark. |

## Explore the project

- [Analysis notebook](EPL_Payroll_Efficiency_2023_24.ipynb) — match checks, payroll cleaning, club comparisons, benchmark and conclusion.
- [Dashboard data](epl_payroll_efficiency_2023_24.csv) — one row per club, with results, payroll and benchmark measures.
- [Tableau workbook](EPL_Payroll_Efficiency_2023_24.twbx) — compare payroll and wins, then select a club to highlight its position in both rankings. Use the payroll-group filter to explore each half of the league.

## Reproduce the analysis

1. Open the notebook in Google Colab. Download the [2023/24 Premier League match file (E0.csv)](https://football-data.co.uk/mmz4281/2324/E0.csv).
2. Run the cells in order. At the upload prompt, choose **E0.csv**. The notebook already contains the historical squad wages table.
3. The notebook checks 380 fixtures, matches wages to all 20 clubs and exports the dashboard CSV.
4. Open the packaged Tableau workbook (`.twbx`) to explore the dashboard. It includes the data extract.

## How to read the numbers

**Cost per win** divides reported annual squad payroll by Premier League wins. **Wins above benchmark** subtracts the wins fitted for that payroll from actual wins. The benchmark is a straight line fitted across all 20 clubs. Selecting a payroll group changes the displayed clubs while preserving the league-wide benchmark.

Both groups had six clubs above benchmark, but the below-median group averaged 0.62 wins below benchmark. The count describes how often clubs beat the benchmark. The average also captures how far each club finished above or below it.

## Sources and scope

Match results come from Football-Data.co.uk. Annual payroll uses the pound amounts in [FBref’s 2023/24 squad wages table, supplied by Capology](https://fbref.com/en/comps/9/2023-2024/wages/2023-2024-Premier-League-Wages). Payroll includes estimates and covers players who also compete outside the league. Points are earned from match results before disciplinary deductions. The model describes this season and was evaluated on the same 20 clubs used to fit it.
