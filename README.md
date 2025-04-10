# Tariff and Economic Data Analysis

This project explores global economic data with a focus on:
1. The relationship between **Trump's alleged tariffs** and **population**.
2. Tariff patterns based on **import values** and other economic indicators.

---

#Datasets Used

### 1. `Tariff_Calculations_plus_Population.csv`
- Columns: Country, US Deficit, US Exports, US Imports, Trump Tariffs Alleged, Trump Response, Population
- Key Features:
  - Tariffs are expressed as percentages
  - Population varies widely, from thousands to billions

### 2. `TariffCalculations.csv`
- Similar to above, without population data
- Useful for additional tariff/deficit/export/import analysis

---

# Data Cleaning Steps
- Removed `%` from percentage fields and converted to numeric
- Removed commas from large numbers (e.g., imports, population)
- Dropped rows with missing or malformed data

---

# Visualizations

### Histogram
- Shows the **distribution of Trump Tariffs Alleged**
- Helpful to see how many countries fall into low, medium, or high tariff categories

### Scatterplot
- Plots **Population (log scale)** vs **Trump Tariffs Alleged**
- Used to explore whether population size correlates with tariff level

---

# Statistical Analysis

### T-Test
- Compares **tariff means** between countries with high vs low import volumes
- Helps determine if there's a significant difference in how tariffs are applied

### Crosstab
- Groups countries by **import tiers** and compares their **tariff level categories**
- Used to examine distribution patterns

---

#Tools & Libraries
- Python (pandas, matplotlib, seaborn, scipy)
- Jupyter Notebook
