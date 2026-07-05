# Token Gateway

A lightweight API gateway that provides access to DeepSeek models via PayPal payments — no Chinese phone number or local payment methods required.

🌐 **Live site:** https://token.mall199.com

## Features

- 🔌 **OpenAI API Compatible** — Use any OpenAI SDK, just change the base URL
- ⚡ **DeepSeek V4 Flash & Pro** — Fast and powerful models
- 💳 **PayPal Payments** — No WeChat, no Alipay, no Chinese phone number
- 🔐 **API Key Authentication** — Secure and trackable usage
- 📊 **Dashboard** — Real-time usage and balance tracking

## Quick Start

```python
from openai import OpenAI

client = OpenAI(
    base_url="https://token.mall199.com/v1",
    api_key="your-api-key-here"
)

response = client.chat.completions.create(
    model="deepseek-flash",
    messages=[{"role": "user", "content": "Hello!"}]
)
print(response.choices[0].message.content)
```

## Pricing

| Model | Input (per 1M tokens) | Output (per 1M tokens) |
|-------|----------------------|-----------------------|
| DeepSeek V4 Flash | $0.50 | $1.00 |
| DeepSeek V4 Pro | $1.50 | $3.00 |

$1 starter package available. No subscription. Balance never expires.

## Tech Stack

- **Backend:** Python (FastAPI)
- **Database:** SQLite
- **Payments:** PayPal REST API
- **Deployment:** VPS + Cloudflare Tunnel

## Project Structure

```
├── app/
│   ├── main.py          # Main application
│   ├── auth.py          # Authentication
│   ├── proxy.py         # API proxy logic
│   ├── payment.py       # PayPal integration
│   ├── db.py            # Database management
│   └── models.py        # Data models
├── static/              # Frontend assets
├── data/                # Configuration
├── Dockerfile
└── requirements.txt
```

## License

MIT
