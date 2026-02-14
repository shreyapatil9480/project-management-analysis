# Project Management Analysis

What inventory conditions cause stockouts?

**Stakeholder:** Inventory Planner

## Key Insights

- Lead times above 14 days raise stockout risk when variability is high.
- Safety stock under 50 units fails for volatile SKUs.
- Demand variability above 0.35 overwhelms default replenishment rules.

## Dataset

Primary file: `data/inventory_stockouts.csv`  
Target variable: `stockout`

## Getting Started

```bash
pip install -r requirements.txt
jupyter notebook notebooks/analysis.ipynb
```


## Next Steps

**Done.** Class-weight tuning and SHAP explainability are implemented — see ### Implemented below.

---
*Analytics portfolio project — 2025-09*

<!-- build 6 -->

### Implemented

```bash
pip install -r requirements.txt
python src/train.py && python src/explain.py
```