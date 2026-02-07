# Phillips Curve: Unemployment vs Inflation (U.S.)

This project analyzes the relationship between unemployment and inflation in the United States using real data from the Federal Reserve (FRED). It visualizes the **Phillips Curve**, a key concept in macroeconomics.

---

## Project Overview
The script:

- Downloads U.S. unemployment data (UNRATE)
- Downloads Consumer Price Index data (CPIAUCSL)
- Calculates monthly inflation
- Plots unemployment vs. inflation as a scatter plot

This allows us to visually examine whether a relationship exists between the two variables.

---

## Data Sources
Data is pulled directly from the Federal Reserve Economic Data (FRED) database:

- **UNRATE**: U.S. Unemployment Rate
- **CPIAUCSL**: Consumer Price Index (All Urban Consumers)

---

## How to Run

### 1. Install dependencies
```bash
py -3 -m pip install -r requirements.txt
2. Run the script
py -3 phillips_curve.py

Methodology

Load unemployment and CPI data from FRED.

Merge both datasets by date.

Compute inflation using:

Inflation = percentage change in CPI


Plot unemployment (x-axis) vs inflation (y-axis).

Results

The scatter plot shows a weak relationship between unemployment and inflation across the full time period.

Points are widely scattered rather than forming a clear downward-sloping line.

This suggests that the traditional Phillips Curve relationship is not consistently strong across decades.

Limitations

Monthly inflation data is noisy.

The relationship between inflation and unemployment changes over time.

Month-to-month CPI changes are less stable than year-over-year inflation.

Future Improvements

Use year-over-year inflation instead of monthly changes.

Split analysis into different time periods.

Add regression lines and correlation statistics.

Test machine learning models to predict inflation.

Example Output

(Add your plot screenshot here)

images/phillips_curve.png

What I Learned

How to load real economic data into Python

How to merge datasets by date

How to compute inflation from CPI

How to visualize economic relationships

Technologies Used

Python

pandas

matplotlib

FRED economic data
