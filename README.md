# Homework 5: Decision Trees, LASSO, PCR and Boosting (DSCI 552)

**Author:** Mohammad Ayaan Khan (GitHub: MohammadAyaanKhan)

## Contents
- `notebook/Khan_MohammadAyaan_HW5.ipynb`: the executed notebook with all code, outputs, plots and written answers.
- `data/`: the two UCI datasets used.
  - `diagnosis.data`, `diagnosis.names`: Acute Inflammations
  - `communities.data`, `communities.names`: Communities and Crime

The notebook reads the data from `../data/` and downloads it from UCI automatically if the files are missing.

## Summary
1. **Decision trees (Acute Inflammations).** All of the 120 patients can be correctly classified by a label-powerset tree with the help of 6 leaves. Through the procedure known as cost-complexity pruning with the one-standard-error rule, the entire tree is kept unchanged, and it can be summarized as two succinct rules. These rules state that nephritis occurs when lumbar pain is present together with temperature higher than 37.95 °C, and bladder inflammation takes place when patients experience urine pushing and (have no lumbar pain or have micturition pain).
2. **Regression (Communities and Crime).** Test MSE: XGBoost with L1 penalty 0.01590, ridge 0.01752, LASSO 0.01768, LASSO on standardized features 0.01772, least squares 0.01797, PCR 0.01837.

## Running
Requires Python 3 with numpy, pandas, matplotlib, seaborn, scikit-learn and xgboost. Open the notebook from the `notebook/` folder and run all cells.
