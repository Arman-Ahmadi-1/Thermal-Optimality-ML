# Thermal-Optimality-ML

Interpretable ML analysis of how **water availability regulates thermal optimality of terrestrial ecosystem productivity** (GPP). This repo contains a cleaned, reproducible notebook (Colab-free paths, repo-relative I/O) with a tiny sample dataset to demonstrate the workflow end-to-end in ~1 minute.

> **Paper:** Ahmadi et al., 2025. *Interpretable Machine Learning Reveals the Crucial Role of Water Availability in Regulating Thermal Optimality of Terrestrial Ecosystems.* JGR: Machine Learning & Computation. https://doi.org/10.1029/2024JH000445

---

## Quickstart

Tested with **Python 3.13** (core stack).  
> Note: For SHAP support, use Python 3.11 (see *Compatibility*).

```bash
# 1) create and activate a local environment
python -m venv .venv
# PowerShell (Windows):
.\.venv\Scripts\activate
# macOS/Linux:
# source .venv/bin/activate

# 2) install deps
python -m pip install --upgrade pip
pip install -r requirements.txt

# 3) run the notebook
# VS Code: open notebooks/ and run cells
# Jupyter: jupyter notebook notebooks/
