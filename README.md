# Drift Monitoring & Feature Analysis

This repository contains a collection of Jupyter notebooks for monitoring **data drift**, **feature drift**, and **distribution shifts** in clinical datasets. The analysis explores correlations between drift metrics and model performance (AUROC), leveraging PCA/TF-IDF methods.

## 📂 Contents

- **baseline_training.ipynb**  
  Trains baseline models for drift monitoring.

- **combined_plot.ipynb**  
  Generates combined visualization plots for multiple drift metrics.

- **Correlation Analysis - Distribution Drift vs Model AUROC.ipynb**  
  Explores the relationship between drift signals and model AUROC performance.

- **drift_visual_v3_training_strategy_feature_investigation.ipynb**  
  Detailed feature-level drift visualization and training strategy experiments.

- **read_data_test.ipynb**  
  Utility notebook for reading and testing datasets.

- **s3_files_download.ipynb**  
  Script for downloading raw data from AWS S3.

- **tfidf_pca.ipynb**  
  Implements TF-IDF with PCA for dimensionality reduction and drift tracking.

## ⚙️ Requirements

- Python 3.8+
- Jupyter Notebook
- Common packages: `numpy`, `pandas`, `matplotlib`, `scikit-learn`, `scipy`, `boto3`

Install dependencies:
```bash
pip install -r requirements.txt
```

## 🚀 Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/<repo-name>.git
   cd <repo-name>
   ```

2. Open Jupyter:
   ```bash
   jupyter notebook
   ```

3. Run the notebooks in order:
   - `s3_files_download.ipynb` → fetch data  
   - `read_data_test.ipynb` → validate data  
   - `baseline_training.ipynb` → train baseline model  
   - `tfidf_pca.ipynb` → perform drift analysis  
   - `combined_plot.ipynb` & `Correlation Analysis...` → visualize and interpret results  

## 📊 Project Context

These notebooks were developed as part of a clinical data science project to evaluate **model robustness under distribution shifts**. Methods include:
- Outlier detection
- Drift monitoring with KS/JS divergence
- PCA-based dimensionality reduction
- Correlation of drift metrics with AUROC
