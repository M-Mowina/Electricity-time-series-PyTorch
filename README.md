# Electricity Consumption Time Series Forecasting

This project implements a time series forecasting model for electricity consumption using PyTorch. The model uses LSTM (Long Short-Term Memory) networks to predict future electricity consumption based on historical data.

## Project Structure

```
.
├── data/
│   └── electricity_consump/
│       └── electricity_train.csv
│       └── electricity_test.csv
├── electricity-consumotion.ipynb
├── requirements.txt
└── README.md
```

## Setup Instructions

1. Create a virtual environment (recommended):
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Launch Jupyter Notebook:
```bash
jupyter notebook
```

4. Open `electricity-consumotion.ipynb` and run the cells sequentially.

## Features

- Data preprocessing and normalization
- LSTM-based time series forecasting model
- Training and evaluation pipeline
- Visualization of results
- Error metrics calculation (MSE, RMSE, MAE, R²)

## Model Architecture

The model uses a 2-layer LSTM network with:
- Input size: 1 (single feature)
- Hidden size: 64
- Number of layers: 2
- Sequence length: 24 hours

## Results

The model's performance is evaluated using:
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- Mean Absolute Error (MAE)
- R-squared Score

Visualizations include:
- Training and testing loss curves
- Actual vs. predicted consumption plots
- Distribution analysis of the consumption data

