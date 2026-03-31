# 📈 Stock News Alert System (Python Automation)

A Python automation project that **monitors stock price movements and sends news alerts via SMS**.

The program checks if a stock price changes significantly between the last two trading days. If the change crosses a defined threshold, it retrieves **recent news articles about the company** and sends them to your phone using **Twilio SMS**.

This project demonstrates **API integration, financial data processing, and automated notifications using Python**.

---

## 🚀 Features

- 📊 Retrieves real-time stock data from Alpha Vantage API
- 📈 Calculates stock price percentage change
- 🔺 Detects upward or downward price movement
- 📰 Fetches latest news related to the company
- 📲 Sends news alerts directly to your phone
- 🔐 Uses Twilio API for SMS notifications
- ⚡ Automated stock monitoring workflow

---

## 🛠 Technologies Used

- Python 3
- Requests (API calls)
- Alpha Vantage API (Stock market data)
- NewsAPI (Latest company news)
- Twilio API (SMS notifications)

---

## 📂 Project Structure

```bash
stockchecker/
│
├── main.py        # Main automation script
├── .gitignore     # Git ignored files
│
└── README.md
```

---

## ⚙️ Requirements

Ensure Python is installed:

```bash
python --version
```

Install required libraries:

```bash
pip install requests twilio
```

---

## 🚀 How to Run the Project

### Clone the Repository

```bash
git clone https://github.com/adebayoadesugba/stockchecker.git
```

### Navigate into the Project Folder

```bash
cd stockchecker
```

### Run the Script

```bash
python main.py
```

---

## 🔑 API Setup

To run this project you need **three APIs**:

### 1️⃣ Alpha Vantage API (Stock Data)

Get a free API key:

```
https://www.alphavantage.co/
```

Replace in code:

```python
STOCK_API_KEY = "YOUR OWN API KEY FROM ALPHAVANTAGE"
```

---

### 2️⃣ News API (News Articles)

Get API key:

```
https://newsapi.org/
```

Replace in code:

```python
NEWS_API_KEY = "YOUR OWN API KEY FROM NEWSAPI"
```

---

### 3️⃣ Twilio API (SMS Alerts)

Create account:

```
https://www.twilio.com/
```

Replace placeholders:

```python
TWILIO_SID = "YOUR TWILIO ACCOUNT SID"
TWILIO_AUTH_TOKEN = "YOUR TWILIO AUTH TOKEN"

VIRTUAL_TWILIO_NUMBER = "your twilio number"
VERIFIED_NUMBER = "your verified phone number"
```

---

## ⚙️ How It Works

1️⃣ The program retrieves **daily stock price data** using Alpha Vantage.

2️⃣ It calculates the **percentage difference between yesterday and the day before yesterday**.

3️⃣ If the change is significant:

```
Stock ↑ or ↓ detected
```

4️⃣ The program fetches **latest news related to the company** using NewsAPI.

5️⃣ The **top 3 news articles** are formatted.

6️⃣ Each article is **sent as an SMS alert** via Twilio.

---

## 📩 Example SMS Alert

```
TSLA: 🔺5%

Headline: Tesla Stock Surges After Earnings

Brief: Tesla shares jumped after reporting stronger-than-expected revenue.
```

---

## 📊 Example Output

```
TSLA: 🔺3%
Headline: Tesla Announces New EV Model
Brief: Tesla revealed its latest electric vehicle with improved battery range.
```

---

## ⚠️ Security Warning

Never expose sensitive information in public repositories.

Do NOT upload:

```
API Keys
Twilio Auth Tokens
Private phone numbers
```

Instead, use:

- Environment variables
- `.env` files
- Secret managers

---

## 🧠 Key Concepts Demonstrated

- API integration
- Financial data analysis
- JSON data processing
- Automation scripting
- Real-time notifications
- SMS integration

---

## 🔮 Future Improvements

- Add support for multiple stocks
- Build a dashboard (React / Flask)
- Add email alerts
- Schedule automated runs (cron jobs)
- Add Telegram / WhatsApp notifications
- Add AI sentiment analysis on news

---

## 👨‍💻 Author

**Adebayo Adesugba**

Full Stack Developer  
Python | JavaScript | React | Node.js | AI Development  

---

## ⭐ Support

If you like this project:

- ⭐ Star the repository
- 🍴 Fork it
- 🧑‍💻 Contribute

---

## 📜 License

This project is open-source and available under the **MIT License**.
