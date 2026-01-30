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
- `index.html` (or `drone-battery-warning-report.html`): full analysis report (exported HTML)

## How to view the report | 如何查看
- Download the HTML and open in a browser (Chrome/Safari).  
- (Optional) Enable **GitHub Pages** for a public web preview:
  1) Keep the report as `index.html`
  2) Repo → Settings → Pages → Deploy from branch (main / root)

## Author
Shu-Yu Lin

