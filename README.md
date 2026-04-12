# Sunspot Cycle Analysis

This repository presents a computational and statistical study of solar activity using Sunspot Number (SSN) data and F10.7 solar radio flux. The project focuses on understanding deviations in Solar Cycle 25 relative to Solar Cycle 24 and evaluating the accuracy of predictive models.

The analysis integrates time-series statistics, regression modeling, and physical interpretation to investigate whether current solar activity aligns with or diverges from established forecasts.

---

## Problem Statement

Most predictive models suggested that Solar Cycle 25 would be weak, similar to Cycle 24. However, real-time observations indicate significantly stronger activity.

This project aims to:

* Quantify the divergence between predicted and observed solar activity
* Identify reliable indicators of real-time solar cycle strength
* Evaluate whether early-cycle growth can predict peak intensity

---

## Objectives

* Compare the rising phases of Solar Cycle 24 and 25
* Estimate growth rates using regression analysis
* Measure structural similarity using correlation
* Perform statistical tests to evaluate significance
* Analyze deviations from predicted models
* Study the relationship between sunspot numbers and F10.7 solar flux
* Visualize solar activity using the butterfly diagram

---

## Repository Structure

```
sunspot-cycle-analysis/
│
├── sunspot_data_preprocessing_and_statistics.ipynb
├── solar_cycle_24_25_comparative_analysis.ipynb
├── sunspot_butterfly_diagram_analysis.ipynb
│
├── datasets/
│   ├── SN_m_tot_V2.0.csv
│   └── fluxtable.csv
│
├── requirements.txt
└── README.md
```

---

## Data Sources

* **SILSO (Sunspot Index and Long-term Solar Observations)**
  Monthly mean sunspot numbers (1749–present, Version 2.0)

* **F10.7 Solar Radio Flux (NOAA)**
  A physical proxy for solar magnetic activity and atmospheric heating

---

## Methodology

### 1. Data Preprocessing

* Clean and format time-series datasets
* Handle missing values
* Align Solar Cycles 24 and 25
* Apply smoothing (rolling averages)

### 2. Rising Phase Analysis

* Analyze first ~60 months of each cycle
* Perform linear regression:

  * Growth rate (slope)
  * Baseline activity (intercept)

### 3. Statistical Analysis

* Pearson correlation for structural similarity
* T-test for statistical significance
* Chi-square test for model comparison
* RMSE and MAE for error evaluation

### 4. Flux–Sunspot Relationship

* Cross-correlation between SSN and F10.7 flux
* Volatility comparison (signal vs noise)

### 5. Butterfly Diagram

* Visualize latitude-time distribution of sunspots
* Observe migration patterns across cycles

---

## Key Results

* **Growth Rate Difference:**
  Cycle 25 grows ~61.6% faster than Cycle 24

* **Cumulative Activity:**
  ~40% more sunspot activity than predicted models

* **Statistical Significance:**
  p-value < 0.05 → difference is statistically significant

* **Correlation:**
  Strong structural similarity (r ≈ 0.85), indicating consistent underlying solar dynamics

* **Flux Insight:**
  F10.7 flux is a more stable and less noisy indicator than sunspot counts

---

## Physical Insight

### Waldmeier Effect

The rise time of a solar cycle is inversely related to its peak amplitude.

→ Faster growth in Cycle 25 implies:

* Higher peak intensity
* Earlier solar maximum

---

## Prediction

Using regression based on historical cycles:

* **Predicted Peak SSN (Cycle 25):** ~183
* **95% Confidence Interval:** ~108 – 258
* Model strength: R² ≈ 0.64

This suggests current models likely underestimate the true intensity of Solar Cycle 25.

---

## Practical Implications

Stronger solar activity can impact:

* Satellite orbits (increased atmospheric drag)
* GPS/GNSS accuracy (ionospheric disturbances)
* Space weather forecasting reliability

---

## Tools & Libraries

* `numpy`
* `pandas`
* `matplotlib`
* `scipy`

---

## How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/sunspot-cycle-analysis.git
   cd sunspot-cycle-analysis
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Update dataset paths if needed:

   ```python
   ssn_path = "datasets/SN_m_tot_V2.0.csv"
   flux_path = "datasets/fluxtable.csv"
   ```

4. Launch Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

---

## Future Work

* Extend analysis to earlier solar cycles
* Apply time-series forecasting models (ARIMA, ML)
* Perform spectral analysis (Fourier/Wavelets)
* Develop interactive visualizations

---

## Authors

* Aparna GR
* Aswathy Sunil
* Aswath Vinod M

BS-MS Physics
IISER Thiruvananthapuram
