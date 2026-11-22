# 📈 Google Stock Price Prediction Using AI

An AI-powered stock price prediction project that uses **Long Short-Term Memory (LSTM)** neural networks to predict Google (GOOGL) stock closing prices based on historical market data.

The project also includes an interactive dashboard for visualizing stock market performance and evaluating the prediction model.

## 🎯 Project Overview

The main goal of this project is to analyze historical Google stock prices and build a deep learning model capable of predicting future closing prices using the previous 60 trading days.

**Dataset:** Google (GOOGL) Historical Stock Data  
**Period:** Last 10 Years  
**Model:** LSTM (Long Short-Term Memory)  
**Framework:** TensorFlow / Keras

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- TensorFlow / Keras
- yfinance
- LSTM Neural Networks

## 🔄 Project Pipeline

The project follows the seven required AI development stages:

1. **Dataset Loading:** Collecting historical Google stock data using Yahoo Finance.
2. **Dataset Exploration:** Analyzing dataset statistics, missing values, and duplicated records.
3. **Dataset Visualization:** Visualizing closing prices, trading volume, and price distribution.
4. **Dataset Preprocessing:** Selecting closing prices, normalizing data, splitting training/testing sets, and creating sequences.
5. **Model Development:** Building and training an LSTM deep learning model.
6. **Model Testing:** Evaluating predictions using MAE, RMSE, and MAPE.
7. **Hyperparameter Tuning:** Comparing different configurations to find the best-performing model.

## 🧠 Model Architecture

The project uses an LSTM neural network with:

- Two LSTM layers.
- Dropout layers to reduce overfitting.
- Dense layers for final prediction.
- Adam optimizer.
- Mean Squared Error (MSE) loss function.

**Input:** Previous 60 trading days.  
**Output:** Predicted next-day closing price.

## ⚙️ Hyperparameter Tuning

Three configurations were tested:

| Configuration | Units | Dropout | Batch Size | Validation Loss |
|---|---:|---:|---:|---:|
| 1 | 32 | 0.2 | 32 | 0.001031 |
| 2 | 50 | 0.2 | 32 | 0.001059 |
| 3 | 64 | 0.3 | 64 | 0.001188 |

**Best Configuration:** Configuration 1.

## 📊 Model Performance

The tuned model achieved the following results on the test dataset:

| Metric | Original Model | Tuned Model |
|---|---:|---:|
| MAE | 26.72 | **25.29** |
| RMSE | 34.82 | **33.25** |
| MAPE | 8.60% | **8.16%** |

The tuned model achieved lower error values across all three evaluation metrics.

## 📉 Interactive Dashboard

The project includes two dashboard views:

### Market Dashboard
- Latest closing price.
- All-time high and low.
- Year-to-date and total returns.
- Average trading volume.
- Moving averages.
- Trading volume visualization.
- 30-day volatility.

### Model Dashboard
- Model evaluation metrics.
- Actual vs. predicted stock prices.
- Prediction error visualization.
- Original vs. tuned model comparison.
- Hyperparameter tuning results.

## 🚀 How to Run

1. Clone this repository:

```bash
git clone https://github.com/YOUR-USERNAME/Google-Stock-Price-Prediction.git
```

2. Navigate to the project directory:

```bash
cd Google-Stock-Price-Prediction
```

3. Install the required libraries:

```bash
pip install yfinance tensorflow scikit-learn pandas numpy matplotlib seaborn
```

4. Open the Jupyter Notebook or Google Colab notebook.

5. Run the cells in order to reproduce the analysis, training, testing, and evaluation.

## ⚠️ Limitations

Stock prices are affected by many external factors that are not included in this model. The model may underpredict sudden price increases and cannot guarantee accurate future predictions.

**This project is for educational purposes only and is not financial advice.**

## 👨‍💻 Team Members

| # | Name | Student ID |
|---|---|---|
| 1 | Adham Mahmoud Saad Mahmoud | 111213 |
| 2 | Ahmed Hany Ismail | 111167 |
| 3 | Ahmed Mohamed Salah Mohamed | 111125 |
| 4 | Ahmed Tarek Hussein Sharaf | 109510 |
| 5 | Adam Medhat Mohamed | 110869 |
| 6 | Salma Emad Ahmed Ibrahim | 109140 |
| 7 | Habiba Mohamed Saeed Hamdaan | 110271 |
| 8 | Ahmed Medhat Abdulla | 110792 |
| 9 | Rawan Salama Farag Tiba | 111271 |

**University:** Modern University for Technology & Information (MTI)  
**Faculty:** Faculty of Computers & AI  
**Course:** Fundamentals of AI  
**Instructor:** Dr. Hesham El-Deeb  
**Teaching Assistants:** Arwa El-Sayed & Gehad Omar

## 📌 Conclusion

This project demonstrates how deep learning, particularly LSTM networks, can be applied to time-series forecasting. It also demonstrates the importance of data preprocessing, model evaluation, and hyperparameter tuning in developing an AI solution.
