# Can Google Trends Data Predict Stock Volatility?

QSS 20 final project (Dartmouth). Ike Mittman and Dyanne Jiang.

## Research question
Do weekly changes in Google search interest for company-specific terms
track, or lead, weekly changes in stock volatility for S&P 500 companies?

## Summary of findings
Changes in search interest are weakly positively correlated with same-week
changes in realized volatility (mean r ≈ 0.05; 70% of companies positive;
~11–12% significant at 5% vs ~5% expected by chance). Lagged search changes
(1–4 weeks) show no consistent lead. See `report/` for the full write-up.

## Repository layout
# FOR SOME REASON THIS LOOKS CONFUSING IN THE README DISLAY BUT WHEN ACTUALLY OPENING THE TEXT IT IS MUCH CLEARER
├── README.md
├── notebooks/
│   ├── finalproject_part1.ipynb
│   └── finalproject_part2.ipynb
├── data/
│   ├── analysis/            # output from finalproject_part1.ipynb
│   ├── analysisfolder/      # output from finalproject_part2.ipynb
│   ├── googletrends/        # output from finalproject_part1.ipynb
│   ├── googletrendsplot/    # output from finalproject_part2.ipynb
│   └── results/             # output from finalproject_part2.ipynb
# descriptions + TF-IDF terms, weekly merged panel
├── figures/            # figures
├── outputs/            # per-company plots
└── report/             # final PDF/LaTeX

## Data sources
- [S&P 500 constituents (Wikipedia)](https://en.wikipedia.org/wiki/List_of_S%26P_500_companies)
- [SEC EDGAR](https://www.sec.gov/edgar) (10-K filings)
- [Google Trends](https://trends.google.com) via `pytrends` (weekly, US, Nov 1 2024 – Nov 1 2026)
- [Yahoo! Finance](https://finance.yahoo.com) via `yfinance` (daily adjusted closes)






