# FinBank Risk Predictor

This repository contains a Jupyter notebook that implements a loan default prediction pipeline using the Kaggle "Give Me Some Credit" dataset and demonstrates synthetic fraud data generation.

Key files:
- `FinBank_Risk_Predictor (2) (1).ipynb` — main analysis notebook
- `cs-training.csv` — dataset (notebook writes embedded copy on first run)
- `requirements.txt` — Python package dependencies

Quickstart
1. Create and activate a Python environment (recommended Python 3.8+).

```bash
python -m venv .venv
# Windows PowerShell
.\.venv\Scripts\Activate.ps1
# or cmd
.\.venv\Scripts\activate.bat
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Open the notebook in Jupyter or VS Code and run cells top-to-bottom. The first cell writes `cs-training.csv` to disk if missing.

Notes
- The notebook trains Logistic Regression, Random Forest and XGBoost models and uses SMOTE for class imbalance.
- For production deployment, export the trained model (`joblib`) and add unit tests and CI.

License
- No license specified. Add a license if you plan to publish.
