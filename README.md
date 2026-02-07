# Phillips Curve Analysis  
### Unemployment vs Inflation in the United States

This project explores the relationship between unemployment and inflation using real economic data from the Federal Reserve (FRED). It visualizes the **Phillips Curve**, a core concept in macroeconomics.

---

## Overview
The script:

- Downloads U.S. unemployment data (UNRATE)
- Downloads Consumer Price Index data (CPIAUCSL)
- Calculates monthly inflation
- Plots unemployment vs. inflation

This allows us to observe whether a relationship exists between the two variables over time.

---

## Data Sources
All data is pulled directly from the Federal Reserve Economic Data (FRED) database:

- **UNRATE** — U.S. Unemployment Rate
- **CPIAUCSL** — Consumer Price Index (All Urban Consumers)

---

## How to Run

### 1. Install dependencies
```bash
py -3 -m pip install -r requirements.txt
py -3 phillips_curve.py
```
## Method

Load unemployment and CPI data from FRED.

Merge datasets by date.

Calculate inflation using CPI percent change.

Plot unemployment (x-axis) vs inflation (y-axis).

### Key Result

The scatter plot shows a weak overall relationship between unemployment and inflation.

Data points form a loose cloud rather than a clear downward slope.

This suggests the Phillips Curve relationship is not consistently strong across the full time period.

## Limitations

Monthly inflation data is noisy.

Economic relationships change over time.

Month-to-month CPI changes are less stable than year-over-year inflation.

# Future Improvements

Use year-over-year inflation instead of monthly changes.

Split analysis by time period.

Add regression line and correlation statistics.

Train a machine learning model to predict inflation.

## Example Output

Add a screenshot of the generated plot here:

images/phillips_curve.png

## What I Learned

Loading real economic data into Python

Merging datasets by date

Calculating inflation from CPI

Visualizing economic relationships

 ### Technologies Used

Python

pandas

matplotlib

FRED economic data
