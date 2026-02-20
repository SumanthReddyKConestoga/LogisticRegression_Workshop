# Logistic Regression Workshop — Spotify Tracks (Explicit vs Non‑Explicit)

A clean, **Week‑6‑aligned** notebook that demonstrates how to frame a real dataset as a **probabilistic binary classification** problem using **Logistic Regression** — with **presentation‑ready EDA**, **advanced evaluation visuals**, and **crisp talking points**.

---

## Business framing (Why this matters) 🎯
In real products, we rarely want only a hard **Yes/No**. We want **risk scores** (probabilities) so we can:
- tune thresholds for different business contexts (e.g., “be stricter for kids mode”),
- measure performance fairly under class imbalance,
- explain decisions to stakeholders.

This workshop turns Spotify track attributes into a model that outputs:
> **P(track is explicit)**

---

## What you will see in the notebook ✅
### 1) Data loading + sanity checks
- shape, missing values, data types
- basic distribution checks for numeric features

### 2) Strong EDA visuals (clean + well‑labeled)
- target balance (% explicit)
- histograms + box/violin‑style comparisons (where relevant)
- feature relationships vs target

### 3) Modeling pipeline (professional, replicable)
- train/test split
- preprocessing for numeric + categorical features (scaling + one‑hot)
- Logistic Regression model in a **scikit‑learn Pipeline**

### 4) Advanced “Week‑6” evaluation visuals 📈
- Confusion Matrix (threshold‑based)
- ROC curve + AUC (threshold‑free ranking)
- Precision‑Recall curve (imbalance‑friendly)
- Calibration curve (probability honesty)
- Threshold sweep plot (tradeoffs)
- Learning curve (data sufficiency / bias‑variance signal)

### 5) Decision boundary / probability surface (visual intuition)
A clearer, more “wow”‑factor visualization showing how probability changes across the feature space.

---

## Repository contents 📦
- `logisticalregression_enhanced.ipynb` — enhanced notebook (final)
- `spotify_tracks.csv` — dataset used by the notebook
- `requirements.txt` — reproducible Python dependencies

---

## Quickstart (Run locally) 🚀

### 1) Create and activate a virtual environment
**Windows (PowerShell)**
```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

**macOS / Linux**
```bash
python3 -m venv .venv
source .venv/bin/activate
```

### 2) Install dependencies
```bash
pip install -r requirements.txt
```

### 3) Launch Jupyter and run the notebook
```bash
jupyter notebook
```
Open:
- `logisticalregression_enhanced.ipynb`

> Tip: Keep `spotify_tracks.csv` in the **same folder** as the notebook for the cleanest run.

---

## Key talking points (presentation‑ready) 🗣️
Use these when presenting:

1. **We turned real music metadata into a yes/no prediction problem**  
   The model learns patterns in popularity, duration, and genre to estimate *how likely a song is explicit*.

2. **Logistic Regression is perfect for Week 6 because it’s explainable**  
   It gives probabilities, supports threshold tuning, and has an interpretable “linear story” in the log‑odds space.

3. **Accuracy alone can lie when classes are imbalanced**  
   Metrics like **log‑loss**, **ROC‑AUC**, and **PR curves** show whether the model is *useful* and *honest*.

---

## Replicability / Testing notes (prof‑proof) 🧪
- The notebook uses:
  - **scikit‑learn Pipelines** to prevent data leakage
  - fixed `random_state` for consistent splits
  - consistent plotting and labeling conventions
- If results differ slightly:
  - confirm same package versions (`pip freeze`)
  - ensure the same CSV is used (no extra preprocessing outside notebook)

---

## Common troubleshooting 🔧
- **FileNotFoundError for CSV**
  - Put `spotify_tracks.csv` next to the notebook
  - Or edit the notebook path cell to point to your local file location

- **Plots not showing**
  - Run the notebook top‑to‑bottom
  - Make sure you’re using Jupyter Notebook/Lab (not a plain .py run)

---



---


