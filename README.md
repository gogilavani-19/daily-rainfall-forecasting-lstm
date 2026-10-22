# daily-rainfall-forecasting-lstm
Daily rainfall prediction using an LSTM deep learning model.
Daily Rainfall Prediction Using LSTM

Project Overview

This project predicts daily rainfall for Coimbatore, Tamil Nadu, using a Long Short-Term Memory (LSTM) neural network.

Dataset

- Source: Kaggle Indian Rainfall Dataset
- Year: 2022
- Location: Coimbatore, Tamil Nadu
- Data: Daily rainfall measurements

Technologies Used

- Python
- Google Colab
- Pandas and NumPy
- TensorFlow and Keras
- Scikit-learn
- Matplotlib

Methodology

1. Load the rainfall dataset.
2. Select Coimbatore district data.
3. Preprocess the data and handle missing values.
4. Normalize rainfall values using MinMaxScaler.
5. Create sequences using the previous seven days to predict the next day.
6. Train an LSTM model.
7. Evaluate predictions using MAE and RMSE.
8. Generate a seven-day experimental forecast.

Model Architecture

- LSTM layer: 32 units
- Dropout: 0.2
- Dense layer: 16 neurons with ReLU
- Output layer: 1 neuron

Results

- MAE: 3.4476
- RMSE: 5.6745

These results are measured on the held-out test data in the dataset's rainfall units. Lower values generally indicate better predictions; comparison with a baseline model is needed to judge performance.

Limitations

The model uses one year of data and rainfall as its only feature. Future predictions are experimental and may not represent actual weather conditions.

How to Run

Open the ".ipynb" notebook in Google Colab and run the cells in order. Upload or configure access to the dataset before running the preprocessing cells.
