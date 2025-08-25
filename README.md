# NYC Restaurant Risk Prediction

## Overview
This project uses NYC restaurant inspection data to train a **Logistic Regression** model that predicts risk categories (**High / Moderate / Low**). The notebook includes **EDA, feature engineering, model training with hyperparameter tuning, and evaluation**. Visualizations highlight borough-level risk distribution and top violation codes.

## Setup

### 1. Clone & environment
```bash
git clone https://github.com/AfonsoVip/NYC-Restaurant-Inspection-Risk-Classification.git
cd NYC-Restaurant-Inspection-Risk-Classification

# create environment
conda create -n nyc-risk python=3.10 -y
conda activate nyc-risk

# install dependencies
pip install -r requirements.txt
```

### requirements.txt
```
pandas
numpy
matplotlib
seaborn
plotly
scikit-learn
jupyter
papermill
```

## Data
Place inspection data in `data/raw/`:
```
data/raw/inspections.csv
```
Adjust the file path in the notebook if your data is stored elsewhere.

## Running

### Interactive
```bash
jupyter lab
# open notebooks/nyc_inspection_model.ipynb
# run all cells
```

### Headless execution
```bash
papermill notebooks/nyc_inspection_model.ipynb \
          outputs/nyc_inspection_model_run.ipynb \

```

## Outputs
- **Classification report** (precision/recall/F1)  
- **Confusion matrix** (PNG, saved under `outputs/figures/`)  
- **High Risk distribution by borough**  
- **Top violation codes** (table/plot)  

## License
MIT
