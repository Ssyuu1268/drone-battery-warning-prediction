# Drone Battery Warning Prediction (Bayesian Network)

## Overview
This project predicts **drone battery warning levels** from sensor data. It combines feature analysis and discretization with a **Bayesian Network** to provide **traceable, probabilistic** early-warning decisions.  

## Problem
- Target: `warning` (multi-class warning level)
- Goal: early detection of high-risk states to reduce operational disruption and safety risk  

## Data & Features
- Correlation analysis to understand sensor relationships and select informative variables  
- Discretization of continuous variables to support BN structure learning  

## Modeling
### 1) Bayesian Network (primary)
- Structure learning: **Hill Climbing** with **K2 score**
- Parameter learning: Bayesian estimator with **BDeu** prior  
→ Outputs warning probabilities for interpretable early-warning decisions.  

### 2) Benchmarks
- **Random Forest** and **XGBoost** for performance comparison  
- Class imbalance handling: **class weighting** and **SMOTE**  

## Deliverables
- `drone_warning_report.html` — full analysis report (exported HTML)

## How to view the report

**Report file:** `drone_warning_report.html`

### Option A (recommended): Open locally
1. Click `drone_warning_report.html` in this repo
2. Click **Download** (or **View raw**)
3. Open the downloaded file with Chrome / Safari

### Option B (optional): GitHub Pages web preview
If you want a shareable web link for the HTML report:
1. (Recommended) rename `drone_warning_report.html` → `index.html`
2. Repo → **Settings** → **Pages**
3. Source: **Deploy from a branch** → Branch: `main` → Folder: `/(root)` → **Save**
4. Open the generated Pages URL (format: `https://<username>.github.io/<repo>/`)


## Use cases (how the results can be used)
- Early-warning alerts for fleet operations to reduce safety risk and downtime.
- Maintenance triage by ranking vehicles/batteries using predicted warning probabilities.
- Explainable diagnostics to support QA reviews and incident post-mortems.


## Author
Shu-Yu Lin

