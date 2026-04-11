
# Solar Cycle Analysis (PHY5132 Project)

This project analyzes solar activity trends using Sunspot Number (SSN) data and solar flux data, with a focus on comparing Solar Cycle 24 and Solar Cycle 25.

The study applies statistical and computational methods to understand the rising phase behavior, correlations, and significance of differences between solar cycles.

---

## Objectives

* Compare the rising phases of Solar Cycle 24 and 25
* Perform linear regression analysis to estimate growth trends
* Measure similarity between cycles using correlation
* Test statistical significance using hypothesis testing
* Analyze residuals and deviations
* Explore relationships between sunspot numbers and solar flux

---

## Data Sources

* Sunspot Number (SSN) Dataset
  Monthly total sunspot numbers from SILSO

* Solar Flux Dataset
  Flux measurements (radio/solar activity proxy)

Note: Update file paths in the code before running (currently set to local directories).

---

## Methods & Analysis

### 1. Data Preprocessing

* Load CSV datasets using `pandas`
* Clean and format time-series data
* Extract relevant cycles and align timelines

### 2. Rising Phase Analysis

* First 60 months of each cycle considered
* Linear regression applied:

  * Slope → growth rate
  * Intercept → baseline activity

### 3. Correlation Analysis

* Pearson correlation coefficient used to compare shape similarity between Cycle 24 and 25

### 4. Statistical Testing

* T-test to check if the two cycles differ significantly
* Chi-square test (manual implementation) for distribution comparison

### 5. Error & Residual Analysis

* RMSE (Root Mean Square Error) used to evaluate fit quality of regression models

### 6. Flux vs Sunspot Comparison

* Merge SSN and flux datasets
* Study relationships between magnetic activity (sunspots) and solar emission (flux)

---

## Tools & Libraries

* `numpy` – numerical computations
* `pandas` – data handling
* `matplotlib` – visualization
* `scipy.stats` – statistical analysis

---

## Key Insights

* Solar Cycle 25 shows comparable but distinct growth behavior relative to Cycle 24
* Correlation varies depending on phase alignment
* Statistical tests help determine whether observed differences are significant
* Flux data provides an additional physical validation of solar activity trends

---

## How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/solar-cycle-analysis.git
   cd solar-cycle-analysis
   ```

2. Install dependencies:

   ```bash
   pip install numpy pandas matplotlib scipy
   ```

3. Update file paths in the notebook:

   ```python
   file_path = 'path_to/SN_m_tot_V2.0.csv'
   flux_file_path = 'path_to/fluxtable.csv'
   ```

4. Run the Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

---

## Project Structure

```
├── PHY5132 Project.ipynb   # Main analysis notebook
├── data/
│   ├── SN_m_tot_V2.0.csv   # Sunspot data
│   └── fluxtable.csv       # Flux data
├── README.md
```

---

## Future Improvements

* Extend analysis to earlier solar cycles
* Apply time-series forecasting models (ARIMA, ML)
* Include spectral analysis (Fourier/Wavelets)
* Improve visualization with interactive plots

---

## Author

Aparna GR
Aswathy Sunil
Aswath Vinod M

BS-MS Physics, IISER Thiruvananthapuram

---
