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

## ⚙️ Installation

1.  **Clone the Repository**

    ``` bash
    git clone https://github.com/Prerna77Arora/Stock_Price_Prediction_Tool.git
    cd Stock_Price_Prediction_Tool
    ```

2.  **Create Virtual Environment**

    ``` bash
    python -m venv venv
    source venv/bin/activate       # macOS/Linux
    venv\Scripts\activate        # Windows
    ```

3.  **Install Requirements**

    ``` bash
    pip install -r requirements.txt
    ```

4.  **Add .env File** Create a `.env` file in the project root with your
    API key:

    ``` env
    NEWS_API_KEY=your_api_key_here
    ```

------------------------------------------------------------------------

## 🧩 Model Training (in Google Colab)

To retrain models: 1. Open `model_training.ipynb` or `train_model.py` in
Google Colab\
2. Train the LSTM model for multiple stocks\
3. The trained `.keras` models and scalers will be saved in `/models`

------------------------------------------------------------------------

## 🖥️ Run the Streamlit App

``` bash
streamlit run app.py
```

Then open the URL shown in your terminal (usually
`http://localhost:8501`).

------------------------------------------------------------------------

## 📊 Example Outputs

-   **Predicted Price:** Model's forecast for next trading day\
-   **Latest Price:** Most recent closing price\
-   **Suggestion:** Buy / Sell / Hold decision based on price change
    threshold

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

## ⚠️ Note

-   `.env` file and model weights are **not included** for security.\
-   Some APIs (like NewsAPI) require an API key.

------------------------------------------------------------------------

## 👩‍💻 Author

**Prerna Arora**\
B.Tech CSE \| Rajiv Gandhi Institute of Petroleum Technology\
GitHub: [@Prerna77Arora](https://github.com/Prerna77Arora)

------------------------------------------------------------------------
