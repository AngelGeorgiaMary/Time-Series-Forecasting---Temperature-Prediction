🌡️ Time Series Forecasting: Melbourne Daily Minimum Temperatures
This project aims to predict daily minimum temperatures in Melbourne using a Long Short-Term Memory (LSTM) neural network. The model leverages historical temperature data to forecast future values, capturing temporal dependencies inherent in time series data.

📂 Dataset
Source: Historical daily minimum temperatures recorded in Melbourne.

Time Frame: 1981 to 1990.

Features:

Date: Observation date.

Temp: Minimum temperature in degrees Celsius.

🛠️ Methodology
Data Preprocessing:

Loaded and visualized the temperature data to understand trends and patterns.

Normalized the temperature values using Min-Max Scaling to bring them into the [0, 1] range.

Created sequences of 30 consecutive days to predict the temperature of the next day.

Model Architecture:

Constructed an LSTM-based neural network with the following layers:

First LSTM layer with 64 units and return_sequences=True.

Second LSTM layer with 32 units.

Dense output layer with 1 unit.

Training:

Compiled the model using the Adam optimizer and Mean Squared Error (MSE) loss function.

Trained the model for 20 epochs with a validation split to monitor performance.

Evaluation:

Plotted training and validation loss over epochs to assess model convergence.

Generated predictions on the test set and compared them against actual values using line plots.

📈 Results
The model effectively captured the temporal patterns in the temperature data, demonstrating its capability in time series forecasting tasks.

📌 Requirements
Ensure the following Python libraries are installed:

pandas

numpy

scikit-learn

tensorflow

matplotlib
