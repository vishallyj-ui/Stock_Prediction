# Stock_Prediction
📈 Stock Price Prediction using LSTM + XGBoost 👨‍💻 Team Members V.C. Prithew Vishallini

📌 Project Overview

This project focuses on predicting stock prices using a hybrid machine learning model that combines:

🔁 LSTM (Long Short-Term Memory) – for capturing time-series patterns ⚡ XGBoost (Extreme Gradient Boosting) – for boosting prediction accuracy

By combining both models, we aim to improve prediction performance compared to using a single model.

🎯 Objectives Predict future stock closing prices Capture temporal dependencies using LSTM Enhance predictions using XGBoost Build a hybrid model for improved accuracy

🧠 Technologies Used Python 🐍 NumPy & Pandas Matplotlib 📊 Scikit-learn TensorFlow / Keras XGBoost

📂 Dataset Dataset used: Ford Stock Prices Contains historical stock data (Close prices used for prediction)

⚙️ Project Workflow

Data Preprocessing Load dataset using Pandas Extract Close price Normalize data using MinMaxScaler
Sequence Creation Convert time-series data into sequences Sequence length used: 150
Model Building
🔁 LSTM Model Two LSTM layers (50 units each) Dense output layer Optimizer: Adam Loss: Mean Squared Error

⚡ XGBoost Model Trees: 500 Learning rate: 0.01 Max depth: 10 5. Hybrid Model

Final prediction is calculated as:Hybrid Prediction = 0.6 * LSTM + 0.4 * XGBoost

📊 Evaluation Metrics Mean Squared Error (MSE) R² Score 📈 Results LSTM captures sequential patterns well XGBoost improves generalization Hybrid model gives better accuracy than individual models

🚀 How to Run the Project

Clone the Repository git clone https://github.com/your-username/stock-prediction.git cd stock-prediction
Install Dependencies pip install numpy pandas matplotlib scikit-learn tensorflow xgboost
Run the Notebook jupyter notebook
Open:PA Project (LSTM + XGBoost).ipynb

📌 Key Features Hybrid ML model (LSTM + XGBoost) Time-series forecasting Data normalization and sequence modeling Performance comparison 🔮 Future Enhancements Use multiple features (Open, High, Low, Volume) Implement real-time prediction Deploy as a web app Hyperparameter tuning 📜 Conclusion

This project demonstrates how combining deep learning and boosting techniques can significantly improve stock price prediction accuracy
