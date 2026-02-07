Title: Phillips Curve: Unemployment vs Inflation (U.S., monthly)

What this does

Downloads U.S. unemployment rate (UNRATE) and CPI (CPIAUCSL) from FRED

Computes monthly inflation from CPI percent change

Plots the Phillips Curve scatter plot

Data Sources

FRED UNRATE (Unemployment Rate)

FRED CPIAUCSL (Consumer Price Index)

How to run

py -3 -m pip install -r requirements.txt
py -3 phillips_curve.py


Method

Merge datasets by date

Compute inflation = pct_change(CPI) * 100

Scatter: Unemployment (x) vs Inflation (y)

Results (what you observed)

The relationship looks weak overall across 1948–present (scatter cloud, not a clear slope)

Limitations

Monthly inflation is noisy

Relationship changes across decades (might be stronger in some eras)

CPI percent change month-to-month isn’t the same as year-over-year inflation

Next improvements

Try year-over-year inflation instead of month-to-month

Split by time periods (ex: 1948–1980 vs 1981–present)

Fit a regression line + report correlation
