# PRCP-1010 — Insurance Claim Prediction (B.Tech Mini Project)

Single-notebook submission for **PRCP-1010-InsClaimPred** (Finance / Insurance).

## What this project does

1. **Task 1:** Predict which customers are likely to file an insurance claim.
2. **Task 2:** Suggestions for the insurance marketing team (risk bands + feature importance).
3. **Model comparison report** across Logistic Regression, Decision Tree, Random Forest, Gradient Boosting, XGBoost, and LightGBM.
4. **Challenges report** with techniques used and reasons.

All of the above live in one notebook:

`PRCP_1010_Insurance_Claim_Prediction.ipynb`

## Dataset

Official Capstone dataset (~595k rows, 59 features, anonymized columns).

- Place file at `Data/train.csv`, **or**
- Open the notebook and run the load cell (it downloads automatically if missing).

Source zip:  
https://d3ilbtxij3aepc.cloudfront.net/projects/CDS-Capstone-Projects/PRCP-1010-InsClaimPred.zip

> `auto_imports.csv` / `auto_imports_names.txt` in the repo are leftover UCI auto-insurance reference files and are **not** used by this notebook.

## Setup

```bash
pip install -r requirements.txt
jupyter notebook PRCP_1010_Insurance_Claim_Prediction.ipynb
```

Optional: set `USE_FULL_DATA = True` in the notebook to train on all rows (slower).

## Outputs

After a successful run:

- `models/best_claim_model.joblib`
- `outputs/model_comparison.csv`
- `outputs/top_features.csv`
- `outputs/risk_segments.csv`
