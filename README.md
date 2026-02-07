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
