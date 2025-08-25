# NYC Restaurant Risk Prediction

## Overview
This project uses NYC restaurant inspection data to train a **Logistic Regression** model that predicts risk categories (**High / Moderate / Low**). The notebook includes **EDA, feature engineering, model training with hyperparameter tuning, and evaluation**. Visualizations highlight borough-level risk distribution and top violation codes.

## Setup

### 1. Clone & environment
```bash
git clone https://github.com/AfonsoVip/NYC-Restaurant-Inspection-Risk-Classification.git

cd NYC-Restaurant-Inspection-Risk-Classification

# create environment, using python 3.9.6 for this build

# First install it through pyenv environment.
pyenv install 3.9.6

# Create environment with python version just downloaded and with structured naming
pyenv virtualenv 3.9.6 nyc-risk

# Activate created env
pyenv activate nyc-risk    

# install dependencies
pip install -r requirements.txt
```

### requirements.txt
```
pandas==2.3.2
numpy==2.0.2
matplotlib==3.9.4
seaborn==0.13.2
plotly==6.3.0
scikit-learn==1.6.1
jupyterlab==4.2.5
notebook==7.2.2
ipykernel==6.30.1
papermill==2.5.0
```

## Data
Place inspection data in `data/raw/`:
```
data/raw/inspections.csv
```

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

## License
MIT
