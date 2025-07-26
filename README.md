# Stock_News_alert_System
# 📈 Tesla Stock News Alert System

This Python script tracks **Tesla Inc. (TSLA)** stock price fluctuations using the Alpha Vantage API and sends news alerts via **Twilio SMS** if the stock changes significantly. It also fetches relevant news from the **NewsAPI** to keep you updated on major company events that might affect the stock.

![Tesla Stock Alert](https://user-images.githubusercontent.com/your-image-link.jpg)

## 🚀 Features

- Fetches **daily stock prices** using the Alpha Vantage API
- Calculates **percentage difference** between last two days' prices
- If price change is significant (e.g., > 5%), fetches top 3 latest **news articles** about Tesla Inc.
- Sends **SMS alerts** using Twilio with the news summary

---

## 🛠️ Technologies Used

- Python
- [Alpha Vantage API](https://www.alphavantage.co/)
- [NewsAPI](https://newsapi.org/)
- [Twilio SMS API](https://www.twilio.com/)

---

## 📦 Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/dhammu10/tesla-stock-alert.git
   cd tesla-stock-alert
# Install dependencies
  pip install requests twilio

# Set up your environment variables (or replace directly in code):
  STOCK_API_KEY=your_alphavantage_api_key
  NEWS_API_KEY=your_newsapi_key
  TWILIO_SID=your_twilio_sid
  TWILIO_AUTH_TOKEN=your_twilio_auth_token
  VIRTUAL_TWILIO_NUMBER=your_twilio_number
  VERIFIED_NUMBER=your_verified_phone_number

## 📋 How It Works
    Script calls Alpha Vantage to get yesterday and day-before stock prices.
    If the difference exceeds 5%, it:
    Fetches top 3 news articles about Tesla
    Formats each article with price change, headline, and summary
    Sends each one via SMS through Twilio

# Sample Output
  TSLA: 🔺6%
  Headline: Tesla stock surges after strong earnings.
  Brief: Tesla shares rose 6% following positive Q2 results and strong delivery numbers.

## 📁 File Structure

      ├── stock_alert.py        # Main script
      └── README.md             # This file


---

Let me know if you’d like this turned into an `.env` version or add an image/logo at the top.


