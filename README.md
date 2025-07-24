# 🤖 Twitter AI Assistant Bot

An intelligent AI-powered Twitter bot that automatically responds to mentions and tweet replies using OpenAI’s GPT model. Ideal for automating engagement, replying smartly, and managing rate limits efficiently.

---

## ✨ Features

- 🔁 **Auto-Reply to Mentions**  
- 💬 **Auto-Reply to Tweet Comments**
- 🧠 **Smart Responses via OpenAI GPT-3.5**
- ⏱️ **Rate Limiting & Daily Tweet Control**
- 📜 **Detailed Logging System**

---

## 🚀 Installation

1. Clone the repository and install the required Python packages:
   ```bash
   pip install -r requirements.txt


## Installation

1. Install the required packages:
```bash
pip install -r requirements.txt
```

2. Create the `.env` file and add the following variables:
```
TWITTER_API_KEY=your_api_key
TWITTER_API_SECRET=your_api_secret
TWITTER_ACCESS_TOKEN=your_access_token
TWITTER_ACCESS_TOKEN_SECRET=your_access_token_secret
TWITTER_BEARER_TOKEN=your_bearer_token
OPENAI_API_KEY=your_openai_api_key
```

## Usage

To start the program:
```bash
python main.py
```

You can choose between two modes:
1. Automatically respond to mentions
2. Automatically respond to comments on tweets

## Project Structure

```
.
├── config/
│   └── config.py         # Konfigürasyon ayarları
├── src/
│   ├── twitter_client.py # Twitter API işlemleri
│   ├── openai_client.py  # OpenAI API işlemleri
│   └── tweet_handler.py  # Tweet işleme mantığı
├── utils/
│   ├── logger.py        # Loglama sistemi
│   └── rate_limiter.py  # Rate limiting işlemleri
├── logs/                # Log dosyaları
├── .env                 # Ortam değişkenleri
├── main.py             # Ana program
└── requirements.txt    # Gerekli paketler
```

## Security

- API keys are securely stored in `.env` file
- API usage is controlled with rate limiting
- Excessive usage is prevented with daily tweet limit

## License

MIT 
