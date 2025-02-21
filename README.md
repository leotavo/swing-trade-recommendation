Swing Trade Recommendation System

👋 Welcome!

This repository contains an AI-based Swing Trade Recommendation System leveraging free APIs, machine learning, and automation to generate trade insights before the market opens.

📌 Project Overview

This project automates swing trade recommendations using:

📊 Financial APIs (BRAPI, Alpha Vantage, Yahoo Finance) for real-time market data.

🤖 Machine Learning (Google Colab) to process historical patterns.

🌍 FastAPI + Render for hosting trade recommendations.

📩 Telegram Bot API for automated notifications.

🚀 Objective: Provide daily buy/sell recommendations based on historical trends and predefined trading strategies.

🛠️ Technologies Used

Python (FastAPI, Pandas, Scikit-Learn, XGBoost)

Google Colab (AI Model Execution)

GitHub Actions (Automated Task Scheduling)

APIs (BRAPI, Alpha Vantage, Yahoo Finance)

FastAPI + Render (Cloud API Deployment)

Telegram Bot API (Automated Trade Alerts)

📂 Project Structure

📂 swing-trade-recommendation/

├── README.md → Documentation & Project Overview
├── colab_script.py → AI Model for Trade Recommendations
├── api.py → FastAPI Service for Fetching Recommendations
├── telegram_bot.py → Script for Sending Telegram Alerts
├── .github/workflows/schedule.yml → GitHub Actions for Automation
└── requirements.txt → Python Dependencies

📌 How It Works

1️⃣ Daily Data Collection - Fetches market data from BRAPI, Alpha Vantage, or Yahoo Finance.2️⃣ Trade Analysis - Runs Machine Learning Models to identify trading opportunities.3️⃣ FastAPI Service - Hosts recommendations via API.4️⃣ Automated Notifications - Sends trade alerts through Telegram Bot API.5️⃣ GitHub Actions - Executes scripts daily before the market opens.

🔧 Installation & Setup

1️⃣ Clone this repository:

git clone https://github.com/YOUR-USERNAME/swing-trade-recommendation.git
cd swing-trade-recommendation

2️⃣ Install dependencies:

pip install -r requirements.txt

3️⃣ Set up Environment Variables:

Create a .env file to store your API keys.

BRAPI_API_KEY=your_api_key
TELEGRAM_BOT_TOKEN=your_bot_token
TELEGRAM_CHAT_ID=your_chat_id

4️⃣ Run the API locally:

uvicorn api:app --host 0.0.0.0 --port 8000

5️⃣ Schedule GitHub Actions for Automation

GitHub Actions will run the AI model daily at 6 AM Brazil Time (UTC-3). You can trigger it manually under Actions.

🚀 Features & Capabilities

✅ Automated Trading Signals (Buy/Sell opportunities)✅ Scheduled Daily Market Analysis✅ FastAPI Web Service for Trade Recommendations✅ Telegram Bot for Instant Trade Alerts✅ Cloud Deployment via Render.com

📊 Sample Trade Recommendation Output

{
    "date": "2024-02-15",
    "recommendations": [
        {
            "stock": "PETR4",
            "action": "BUY",
            "entry_price": 28.50,
            "stop_loss": 27.93,
            "take_profit": 29.07
        },
        {
            "stock": "VALE3",
            "action": "SELL",
            "entry_price": 98.00,
            "stop_loss": 99.96,
            "take_profit": 96.04
        }
    ]
}

📩 How to Receive Trade Alerts

1️⃣ Set up a Telegram Bot via BotFather.2️⃣ Get your BOT TOKEN & CHAT ID and add them to .env.3️⃣ Run the bot manually:

python telegram_bot.py

🚀 Next Steps & Improvements

✅ Add Backtesting Capabilities to validate strategies.
✅ Improve Machine Learning Algorithms for trade predictions.
✅ Create a Web Dashboard for real-time trade tracking.

📬 Contact & Contribution

👨‍💻 Developed by Leonardo Trindade📧 Email: leotavo@gmail.com
🔗 LinkedIn: [Leonardo Trindade](https://www.linkedin.com/in/leotavo/)

🙌 Contributions are welcome! Feel free to fork, improve, and submit pull requests.
