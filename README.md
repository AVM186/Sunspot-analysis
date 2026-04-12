# Sunspot Cycle Analysis

This repository presents a computational study of solar activity using Sunspot Number (SSN) data and solar flux measurements. The project focuses on understanding temporal patterns in solar cycles, with particular emphasis on Solar Cycle 24 and Solar Cycle 25.

The workflow is structured as a pipeline: data preprocessing, statistical analysis of solar cycles, and physical visualization using the butterfly diagram.

---

## Objectives

* Analyze long-term trends in sunspot activity
* Compare the rising phases of Solar Cycle 24 and 25
* Quantify growth using regression techniques
* Measure similarity between cycles using correlation
* Evaluate statistical significance of observed differences
* Study the relationship between sunspot number and solar flux
* Visualize spatiotemporal evolution of sunspots using the butterfly diagram

---

## Repository Structure

```
sunspot-cycle-analysis/
│
├── sunspot_data_preprocessing_and_statistics.ipynb
├── solar_cycle_24_25_comparative_analysis.ipynb
├── sunspot_butterfly_diagram_analysis.ipynb
│
├── data/
│   ├── SN_m_tot_V2.0.csv
│   └── fluxtable.csv
│
└── README.md
```

---

## Data Sources

* **Sunspot Number (SSN):**
  Monthly total sunspot numbers from SILSO

* **Solar Flux Data:**
  Radio flux measurements as a proxy for solar activity

> Note: Update file paths in the notebooks before execution.

---

## Methodology

### 1. Data Preprocessing & Exploration

* Import and clean datasets using `pandas`
* Construct time-series format
* Handle missing values and align datasets

### 2. Solar Cycle Comparison

* Extract and align rising phases (first ~60 months)
* Apply linear regression:

  * Slope → growth rate
  * Intercept → baseline activity
* Compute Pearson correlation to compare cycle shapes

### 3. Statistical Analysis

* Perform hypothesis testing (t-test)
* Compare distributions using chi-square test
* Evaluate model performance using RMSE

### 4. Flux–Sunspot Relationship

* Merge SSN and flux datasets
* Analyze correlation between magnetic activity and solar emission

### 5. Butterfly Diagram Analysis

* Visualize sunspot latitude vs time
* Capture migration of solar activity bands across cycles
* Provide a physical interpretation of solar cycle evolution

---

## Tools & Libraries

* `numpy` — numerical computation
* `pandas` — data processing
* `matplotlib` — visualization
* `scipy.stats` — statistical analysis

---

## Key Insights

* Solar Cycle 25 exhibits growth behavior comparable to, but distinct from, Cycle 24
* Correlation between cycles depends strongly on phase alignment
* Statistical tests provide insight into the significance of differences
* Solar flux acts as an independent validation of activity trends
* Butterfly diagrams reveal the latitudinal migration of sunspot activity over time

---

## How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/sunspot-cycle-analysis.git
   cd sunspot-cycle-analysis
   ```

2. Install dependencies:

   ```bash
   pip install numpy pandas matplotlib scipy
   ```

3. Update dataset paths inside notebooks:

   ```python
   ssn_path = "path_to/SN_m_tot_V2.0.csv"
   flux_path = "path_to/fluxtable.csv"
   ```

4. Launch Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

---

## Future Work

* Extend analysis to multiple historical solar cycles
* Apply time-series forecasting models (ARIMA, ML approaches)
* Perform spectral analysis (Fourier / Wavelet methods)
* Develop interactive visualizations

---

## Authors

* Aparna GR
* Aswathy Sunil
* Aswath Vinod M

BS-MS Physics
IISER Thiruvananthapuram
