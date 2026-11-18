# 📈 Stock Prediction Tool

An AI-powered stock price prediction app built using **Streamlit**,
**LSTM neural networks**, and **sentiment analysis** from news, Twitter,
and Google Trends data.

------------------------------------------------------------------------

## 🧠 Overview

This tool predicts the **next day's stock price** using: - Historical
price data (via Yahoo Finance) - News sentiment (via FinBERT) - Twitter
sentiment (via VADER) - Google Trends data

The model is trained in Google Colab and integrated into the Streamlit
app for live inference.

------------------------------------------------------------------------

## 🏗️ Project Structure

    stock_tool/
    ├── app.py                   # Streamlit frontend + backend integration
    ├── backend/
    │   ├── stock_data.py        # Fetch stock data from Yahoo Finance
    │   ├── sentiment.py         # Fetch sentiment data from news, twitter, google trends
    │   ├── features.py          # Feature engineering for ML model
    │   ├── model.py             # LSTM model prediction handler
    │   ├── train_model.py       # Model training (Google Colab)
    ├── data/
    │   ├── stock_list.csv       # List of stocks with ticker and sector
    ├── models/                  # Saved trained models and scalers
    ├── .env                     # API keys and secrets (NOT uploaded to GitHub)
    ├── requirements.txt         # Dependencies
    └── README.md

------------------------------------------------------------------------

## 🚀 Features

✅ Predicts next-day stock price using LSTM model\
✅ Integrates FinBERT & VADER for sentiment analysis\
✅ Uses Google Trends for trend-based features\
✅ Sector-wise stock filtering\
✅ Provides Buy/Sell/Hold recommendation\
✅ Interactive Streamlit dashboard with charts

------------------------------------------------------------------------


## 🧠 Technologies Used

-   Streamlit\
-   TensorFlow / Keras\
-   Scikit-learn\
-   yFinance\
-   FinBERT (Transformers)\
-   VADER Sentiment Analyzer\
-   Google Trends API\
-   Plotly for visualization

------------------------------------------------------------------------

