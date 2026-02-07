# Phillips Curve Analysis  
### Unemployment vs Inflation in the United States

This project explores the relationship between unemployment and inflation using real economic data from the Federal Reserve (FRED). It visualizes the **Phillips Curve**, a core concept in macroeconomics.

---

## Overview
The script:

- Downloads U.S. unemployment data (**UNRATE**)
- Downloads Consumer Price Index data (**CPIAUCSL**)
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
```

### 2. Run the script
```bash
py -3 phillips_curve.py
```

---

## Method
1. Load unemployment and CPI data from FRED.
2. Merge datasets by date.
3. Calculate inflation using CPI percent change.
4. Plot unemployment (x-axis) vs inflation (y-axis).

---

## Key Result
- The scatter plot shows a **weak overall relationship** between unemployment and inflation.
- Data points form a loose cloud rather than a clear downward slope.

This suggests the Phillips Curve relationship is not consistently strong across the full time period.

---

## Limitations
- Monthly inflation data is noisy.
- Economic relationships change over time.
- Month-to-month CPI changes are less stable than year-over-year inflation.

---

## Future Improvements
- Use year-over-year inflation instead of monthly changes.
- Split analysis by time period.
- Add regression line and correlation statistics.
- Train a machine learning model to predict inflation.

---

## Example Output

<img width="794" height="601" alt="image" src="https://github.com/user-attachments/assets/f129fb55-6ff5-4cf1-a7ad-b887d0d1f58e" />


---

## What I Learned
- Loading real economic data into Python
- Merging datasets by date
- Calculating inflation from CPI
- Visualizing economic relationships

---

## Technologies Used
- Python 3.14.2
- pandas
- matplotlib
- FRED economic data
