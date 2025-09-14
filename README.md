# Thermal-Optimality-ML

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

Interpretable machine learning framework for analyzing how **water availability regulates thermal optimality of terrestrial ecosystem productivity (GPP)**. This repo contains cleaned, reproducible code from:

> **Ahmadi et al., 2025** – *Interpretable Machine Learning Reveals the Crucial Role of Water Availability in Regulating Thermal Optimality of Terrestrial Ecosystems.*  
> Journal of Geophysical Research: Machine Learning and Computation.  
> [Paper Link (Open Access)](https://doi.org/10.1029/2024JH000445)

---

## 🚀 Quickstart

Tested with **Python 3.13** (core stack).  

```bash
# 1) Create and activate a local environment
python -m venv .venv
# PowerShell (Windows):
.\.venv\Scripts\activate
# macOS/Linux:
# source .venv/bin/activate

# 2) Install dependencies
python -m pip install --upgrade pip
pip install -r requirements.txt

# 3) Run the notebook
# VS Code: open notebooks/ and run cells
# Jupyter: jupyter notebook notebooks/
```
Expected runtime: ~1 minute with sample data.


## 📂 Repository Structure

```
thermal-optimality-ml/
│
├── data/
│   └── sample/                   <- sample CSVs for quick demo (two AmeriFlux sites)
│
├── notebooks/
│   └── 00_research_archive.ipynb <- original analysis notebook (Colab, extra cells & details)
│   └── 01_quickstart.ipynb       <- reproducible notebook
│
├── outputs/                      <- generated artifacts for the demo run
│
├── src/                          <- placeholder – future refactor of helper functions
├── docs/                         <- placeholder – project documentation
├── tests/                        <- placeholder – future unit tests
│
├── requirements.txt              <- dependencies
├── LICENSE
└── README.md
```

## 📊 What’s Inside
The sample notebook demonstrates:

- Loading & preprocessing flux data
- Exploratory data analysis and visualization
- Interpretable ML (XGBoost, PDP, ALE)
- Trend analysis of ERA5 data
- Thermal acclimation analysis

> For full-scale experiments and exact figures in the paper, follow the methods and data sources described in the manuscript.

## 📁 Data
- This repo includes only two AmeriFlux sites in data/sample/ to ensure reproducibility.
- Full data (AmeriFlux & ERA5) must be obtained from their original sources (links in the paper).
- Replace data/sample/sites and /ERA5 with the full dataset to reproduce paper-level results.

## ⚙️ Environment & Compatibility
- **Primary:** Python 3.13, core stack (numpy, pandas, scikit-learn, matplotlib, seaborn, math).
- **ML & Interpretation:** xgboost, optuna, PyALE
- **Trend Analysis:** pymannkendall

## 📖 Citation

If you use this repository or build upon the methods, please cite:

> Ahmadi, A., Mallick, K., Yi, K., & Baldocchi, D. (2025). Interpretable machine learning reveals the crucial role of water availability in regulating thermal optimality of terrestrial ecosystems. *Journal of Geophysical Research: Machine Learning and Computation.*
https://doi.org/10.1029/2024JH000445

**BibTeX**
```bibtex
@article{Ahmadi2025-Thermal-Optimality-ML,
  author  = {Ahmadi, Arman and Mallick, Kanishka and Yi, Koong and Baldocchi, Dennis},
  title   = {Interpretable Machine Learning Reveals the Crucial Role of Water Availability in Regulating Thermal Optimality of Terrestrial Ecosystems},
  journal = {Journal of Geophysical Research: Machine Learning and Computation},
  year    = {2025},
  volume  = {2},
  pages   = {e2024JH000445},
  doi     = {10.1029/2024JH000445}
}
```

## 📜 License
Licensed under the [MIT License](LICENSE).

## ✉️ Contact
**Arman Ahmadi**  
📧 a.ahmadi@berkeley.edu  
🔗 [LinkedIn](https://www.linkedin.com/in/arman-ahmadi/) · [Google Scholar](https://scholar.google.com/citations?user=oRpYGmIAAAAJ&hl=en&oi=ao)
