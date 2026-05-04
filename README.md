📈 LSTM Stock Price Prediction (Tesla Dataset)
📌 Project Overview

This project demonstrates the use of Long Short-Term Memory (LSTM) networks for predicting stock prices using deep learning.

The model is trained on historical Tesla stock price data and learns temporal patterns to predict future closing prices. This project highlights how Recurrent Neural Networks (RNNs) can be applied to real-world financial forecasting.
.

🎯 Objective
Analyze historical Tesla stock price data
Perform time series preprocessing
Build and train an LSTM model
Predict future stock prices
Visualize actual vs predicted results
📂 Dataset
📊 Dataset: Tesla Stock Price Dataset
🔗 Source: Kaggle

📥 Loaded via:

https://raw.githubusercontent.com/plotly/datasets/master/tesla-stock-price.csv
Features Used:
Close Price (primary feature used for prediction)

Technologies & Libraries
Python 🐍
NumPy
Pandas
Matplotlib
Scikit-learn
TensorFlow / Keras

Project Workflow
1. Data Collection
Loaded Tesla dataset from online source
2. Exploratory Data Analysis (EDA)
Visualized historical stock prices using line plots
3. Data Preprocessing
Selected Close price
Applied MinMaxScaler (0–1 normalization)
Created sequences of 60 days for time series prediction
Split dataset:
80% Training
20% Testing

4. Model Architecture
Sequential Deep Learning Model:
LSTM Layer (50 units, return_sequences=True)
Dropout (0.2)
LSTM Layer (50 units)
Dropout (0.2)
Dense Layer (25 neurons)
Output Layer (1 neuron)
Compilation:
Optimizer: Adam
Loss Function: Mean Squared Error
5. Model Training
Batch Size: 32
Epochs: 10

6. Prediction
Prepared test dataset
Generated predictions using trained model
Applied inverse scaling to get actual values
7. Visualization

The model performance is visualized using:

Training data
Actual stock prices
Predicted stock prices

📊 The graph shows how closely the predicted values follow actual trends.

📊 Results
The model successfully captures stock price trends
Predictions are close to actual values
Performance depends on:
Sequence length
Training epochs
Data quality
📷 Output Screenshots

(Add these images in your repo)

📈 Stock Price History Graph
📉 Prediction vs Actual Graph
🚀 How to Run the Project
# Clone the repository
git clone https://github.com/your-username/lstm-stock-price-prediction.git

# Navigate to project folder
cd lstm-stock-price-prediction

# Install required libraries
pip install numpy pandas matplotlib scikit-learn tensorflow

# Run Jupyter Notebook
jupyter notebook
📌 Future Improvements
Use multiple features (Open, High, Low, Volume)
Apply GRU / Transformer models
Increase epochs for better accuracy
Hyperparameter tuning
Deploy using Streamlit
🎓 Conclusion

This project demonstrates how LSTM networks can effectively model time-series data like stock prices. It provides a strong foundation for financial forecasting using deep learning techniques.
