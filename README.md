# Solar Cycle Analysis (PHY5132 Project)

This project analyzes solar activity trends using Sunspot Number (SSN) and solar flux data, with a focus on comparing **Solar Cycle 24** and **Solar Cycle 25**.

The work applies statistical and computational methods to study growth behavior, correlations, and the significance of differences between the two cycles.

---

## Objectives

* Compare the rising phases of Solar Cycle 24 and 25
* Estimate growth trends using linear regression
* Measure similarity using correlation
* Test statistical significance (t-test, chi-square)
* Analyze residuals and model deviations
* Study relationship between sunspots and solar flux

---

## Data Sources

* **Sunspot Number (SSN):** Monthly data from SILSO
* **Solar Flux:** Radio flux as a proxy for solar activity

All datasets are stored in the `datasets/` folder.

---

## Methods

* Data preprocessing and cycle alignment
* Rising phase extraction (first 60 months)
* Linear regression (slope → growth rate)
* Pearson correlation analysis
* Hypothesis testing (t-test, chi-square)
* RMSE for fit evaluation
* Flux vs SSN comparison

---

## Tools & Libraries

* `numpy`
* `pandas`
* `matplotlib`
* `scipy`

---

## Key Insights

* Solar Cycle 25 shows comparable but distinct growth behavior relative to Cycle 24
* Correlation depends on phase alignment
* Statistical tests help assess significance of differences
* Flux data supports trends observed in sunspot activity

---

## Project Structure

```
├── PHY5132 Project.ipynb
├── Butterfly_Final.ipynb
├── phy5132-solar-cycle-analysis-presentation.pptx
├── datasets/
│   ├── SN_m_tot_V2.0.csv
│   └── fluxtable.csv
├── README.md
```

---

## How to Run

```bash
git clone https://github.com/your-username/solar-cycle-analysis.git
cd solar-cycle-analysis
pip install numpy pandas matplotlib scipy
jupyter notebook
```

Update dataset paths inside the notebook if required.

---

## Presentation

* Download: `phy5132-solar-cycle-analysis-presentation.pptx`

---

## Future Work

* Extend analysis to earlier solar cycles
* Apply time-series forecasting (ARIMA / ML)
* Perform spectral analysis (Fourier / wavelets)
* Improve visualization and interactivity

---

## Authors

* Aparna GR
* Aswathy Sunil
* Aswath Vinod M

BS-MS Physics, IISER Thiruvananthapuram

