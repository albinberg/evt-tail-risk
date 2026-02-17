# Extreme Value Theory Analysis of Equity Returns

This project applies **Extreme Value Theory (EVT)** to historical equity return data in order to model **tail risk** and study the behavior of extreme downside events in financial markets.

The analysis is implemented in **Python** using scientific computing and statistical libraries, with a focus on fitting the **Generalized Pareto Distribution (GPD)** to exceedances over high thresholds.

# Background
I took a course at Chalmers on extreme value theory in the spring of 2026 which sparked my interest in applications within this field. Deriving the distributions used in this project is not a trivial task, one I won't bore you with here. In essence, the entire field stems from dutch mathematichians having an interest in statistics on the sea level, not just on the average like the regular statistics show, but in extreme cases where large parts of the country might end up under water. This led to the development of the extreme value theory in mathematics and it has proven useful in financial modelling among other things. 

---

## Objectives

* Estimate tail risk in equity returns using EVT methods
* Fit **Generalized Pareto** models to extreme negative returns
* Evaluate **threshold stability** and **mean excess functions**
* Visualize return distributions and extreme-value diagnostics

---

## Methods

The workflow follows a classical **Peaks-Over-Threshold (POT)** EVT approach:

1. Download and preprocess historical price data
2. Compute log-returns and isolate negative tail observations
3. Select high thresholds using quantile grids
4. Fit **GPD parameters** via maximum likelihood estimation
5. Analyze:

   * Shape parameter stability
   * Scale parameter behavior
   * Mean residual life plots
6. Interpret implications for **extreme downside risk**

---

## Technologies Used

* **Python**
* **NumPy, Pandas**
* **SciPy (genpareto)**
* **Matplotlib**
* **Jupyter Notebook**

---

## Project Structure

```
evt-tail-risk/
│
├── evt_analysis.ipynb      # Main EVT analysis notebook
├── requirements.txt        # Python dependencies
└── README.md
```

---

## How to Run

Clone the repository and install dependencies:

```bash
git clone https://github.com/albinberg/evt-tail-risk.git
cd evt-tail-risk
pip install -r requirements.txt
```

Launch the notebook:

```bash
jupyter notebook evt_analysis.ipynb
```

---

## Results & Insights

The EVT framework enables:

* Quantification of **extreme downside risk**
* Statistical modeling beyond normal-distribution assumptions
* Insight into **tail heaviness** of equity return distributions

This type of analysis is relevant for:

* **Risk management**
* **Quantitative finance**
* **Stress testing and scenario analysis**

---

## Future Improvements

Possible extensions include:

* Value-at-Risk (VaR) and Expected Shortfall estimation using EVT
* Comparison across multiple equities or indices
* Rolling-window tail risk dynamics
* Integration with portfolio optimization or ML-based volatility models

---

## Author

**Albin Berg**
Industrial Engineering student, Chalmers University of Technology
Prospective M.Sc. in Data Science and AI
GitHub: https://github.com/albinberg
