# Phillips Curve Analysis

An economic data analysis project examining the relationship between unemployment and inflation using real Federal Reserve data.

## Overview

The Phillips Curve is one of the most important concepts in macroeconomics, suggesting an inverse relationship between unemployment and inflation. This project tests this theoretical relationship using actual U.S. economic data from FRED (Federal Reserve Economic Data).

## What It Does

- Pulls real unemployment data from FRED (U.S. Bureau of Labor Statistics)
- Pulls real inflation data from FRED (Consumer Price Index)
- Merges the datasets by date
- Creates a scatter plot visualization showing the relationship
- Analyzes whether the theoretical inverse relationship holds in real data

## The Phillips Curve Theory

**Traditional theory states:**
- When unemployment is LOW → inflation tends to be HIGH
- When unemployment is HIGH → inflation tends to be LOW

**This is because:**
- Low unemployment = tight labor market = higher wages = higher prices
- High unemployment = slack labor market = lower wages = lower prices

## What the Data Shows

The scatter plot reveals that the Phillips Curve relationship is more complex in modern data than the simple theory suggests. The data points show significant scatter, indicating that other factors beyond unemployment also drive inflation.

## Technical Details

**Data Sources:**
- Unemployment Rate (UNRATE) - Federal Reserve Economic Data
- Consumer Price Index (CPIAUCSL) - Federal Reserve Economic Data
- Time period: 2026

**Tools Used:**
- Python 3.14.2
- pandas - Data manipulation and analysis
- matplotlib - Data visualization
- FRED API - Federal Reserve economic data

## Code Structure
```python
# Pull unemployment data
unemployment_url = "https://fred.stlouisfed.org/graph/fredgraph.csv?id=UNRATE"
unemployment = pd.read_csv(unemployment_url)

# Pull inflation data
inflation_url = "https://fred.stlouisfed.org/graph/fredgraph.csv?id=CPIAUCSL"
inflation = pd.read_csv(inflation_url)

# Merge and analyze
# Create scatter plot visualization
```

## Key Findings

[Add your observations here - for example:]
- The relationship shows significant scatter rather than a clear inverse correlation
- Modern data suggests the Phillips Curve may have "flattened" over time
- Multiple factors influence inflation beyond just unemployment
- Useful for understanding macroeconomic policy trade-offs

## What I Learned

- How to access and use Federal Reserve economic data
- Data merging and manipulation with pandas
- Statistical analysis and correlation
- Economic data visualization techniques
- The complexity of real-world economic relationships vs. theoretical models
- How central banks (like the Fed) use these relationships for policy decisions

## Applications

This analysis is relevant for:
- Understanding Federal Reserve monetary policy decisions
- Economic forecasting and analysis
- DECA competition preparation (macroeconomics knowledge)
- Research into macroeconomic relationships

## Future Improvements

- [ ] Add time-series analysis to see how the relationship has changed over decades
- [ ] Include additional variables (money supply, GDP growth)
- [ ] Create interactive dashboard version
- [ ] Add statistical correlation coefficient
- [ ] Segment by different time periods (pre-1980s vs post-1980s)
- [ ] Compare U.S. data to other countries

## Part of AI×Economics Portfolio

This project demonstrates the application of data science techniques to economic analysis, making complex macroeconomic concepts accessible through visualization and real data.

**Project #8** - February 2026

---

## Usage
```bash
python phillips_curve.py
```

The script will automatically pull the latest data from FRED and generate the scatter plot visualization.

## Requirements
```
pandas
matplotlib
```

Install with:
```bash
pip install pandas matplotlib
```

## About

Built while learning economic data analysis and exploring the intersection of AI, data science, and economics. Part of preparation for DECA competitions and future economics research.
