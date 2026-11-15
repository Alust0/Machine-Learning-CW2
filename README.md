# Machine Learning Coursework 2 (6001CEM)

Predictive modeling and end-to-end consultancy project on the **Default of Credit Card Clients** dataset (Taiwan, 2005).

---

## Project Structure (Tasks A to D)

All code and analytical experiments are structured into four dedicated Jupyter notebooks named in PascalCase without spaces or underscores:

1. **`PartAProblemAnalysis.ipynb`** (10 Marks)
   - Business background, problem formulation, feature taxonomy, target variable analysis, and technical justification for Classification.
2. **`PartBComparativeAnalysis.ipynb`** (10 Marks)
   - Supervised vs. Unsupervised comparative analysis with empirical K-Means vs. Logistic Regression experimental proof.
3. **`PartCEDAInvestigation.ipynb`** (10 Marks)
   - Descriptive statistics, correlation heatmaps, skewness, outlier boxplots, duplicate analysis, and model impact.
4. **`PartDDataPreparationFeatureEngineering.ipynb`** (15 Marks)
   - Full 12-step data pipeline: duplicate removal, categorical recoding, feature engineering, scaling, feature selection, PCA evaluation, and SMOTE balancing.

---

## Running with Docker (No Local Setup Required)

Anyone with [Docker Desktop](https://www.docker.com/products/docker-desktop/) installed can run all four notebooks with a single command:

### 1. Start the Environment
```bash
docker compose up
```

### 2. Open Jupyter in Browser
Navigate to:
```
http://localhost:8888
```
All libraries (`pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`, `imbalanced-learn`, `jupyter`) are pre-installed. All edits and exported CSVs sync live with your computer.

### 3. Stop the Container
```bash
docker compose down
```

---

## Running Locally with Python

```bash
# 1. Create and activate virtual environment
python -m venv .venv
.\.venv\Scripts\Activate.ps1    # On Windows PowerShell

# 2. Install dependencies
pip install -r requirements.txt

# 3. Launch Jupyter
jupyter notebook
```
