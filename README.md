# Energy Forecasting and Anomaly Detection for Industrial Consumption

This repository contains my capstone project work on two connected tasks:

1. Energy consumption forecasting for industrial datasets.
2. Energy anomaly detection for unusual usage patterns.

The project is implemented primarily in Jupyter notebooks and includes both exploratory iterations and final model versions.

## Project Goals

- Build practical energy forecasting workflows for real-world industrial data.
- Detect abnormal consumption events to support operational monitoring.
- Compare model behavior across two datasets:
  - Crown Paper Mill (CPM)
  - Steel Industry

## Repository Structure

The workspace includes development history and final deliverables.

### Main folders

- 1- Time Series Forecast Code/
  - Forecasting notebooks and related CSV/XLSX files
- 2- Anomaly Detection Code/
  - Anomaly detection notebooks and source datasets
- 3- Final Codes/
  - Consolidated final notebooks
  - 1- Energy Forecast Models/
  - 2- Energy Anomaly Detection Models/

### Final notebooks to start with

- 3- Final Codes/Energy Forecast_CPM_Final.ipynb
- 3- Final Codes/Anomaly_Detection_model_CPM_Final.ipynb
- 3- Final Codes/1- Energy Forecast Models/Energy Forecast_Steel_Industry_Final.ipynb
- 3- Final Codes/2- Energy Anomaly Detection Models/Anomaly_Detection_model_Steel_Industry_Final.ipynb

## Data

The project includes industrial energy files such as:

- Copy of Consumption Dashboard_CROWN PAPER MILL LTD._ (002).csv
- First_Dataset_Steel_Industry_data.csv
- Historical_Pred_df_Energy_Consumption_CPM.csv
- Historical_Pred_df_Energy_Usage.csv

## Anomaly Detection Approach

The anomaly detection workflow in this repository combines:

- Data preprocessing and feature preparation with pandas and numpy
- Rule-based anomaly labeling from energy usage behavior
- Deep learning experiments for anomaly classification (including Conv1D/CNN-style and recurrent layers)
- Model evaluation through confusion matrices and classification metrics
- Visualization with matplotlib and seaborn

Core libraries used in notebooks include:

- pandas, numpy
- matplotlib, seaborn
- scikit-learn
- tensorflow/keras
- xgboost (in selected experiments)

## Getting Started

### 1. Clone the repository

Use your Git client to clone this repo locally.

### 2. Create and activate a Python environment

Recommended Python version: 3.9 to 3.11

Example with conda:

```bash
conda create -n energy-ml python=3.10 -y
conda activate energy-ml
```

### 3. Install dependencies

```bash
pip install jupyter pandas numpy matplotlib seaborn scikit-learn tensorflow xgboost
```

### 4. Launch Jupyter

```bash
jupyter notebook
```

Then open the final notebooks listed above.

## Notes on Reproducibility

- Some notebooks currently reference absolute local paths from development.
- If a notebook fails to load data, update file paths to relative paths in your local clone.
- Several notebooks are preserved as working history copies (Copy1, Copy2, etc.) for traceability.

## Suggested Execution Order

1. Run final forecasting notebooks in 3- Final Codes/1- Energy Forecast Models/
2. Run final anomaly notebooks in 3- Final Codes/2- Energy Anomaly Detection Models/
3. Compare model behavior between CPM and Steel Industry datasets

## Current Status

- Forecasting models: implemented and archived in final notebooks
- Anomaly detection models: implemented with deep learning experiments and evaluation outputs
- Repository cleanup: pending reduction of duplicate notebook versions and path normalization

## Future Improvements

- Convert all notebook file paths to fully relative paths
- Add a requirements.txt and environment.yml for one-command setup
- Export key model artifacts and add a lightweight inference script
- Add an optional dashboard for anomaly monitoring

## Author

Hasan Jadallah

## License

No license file is currently provided. Add a LICENSE file if you want to define reuse terms.
