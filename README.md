# Token Gateway — DeepSeek API via PayPal (No Chinese Phone Required)

<img width="1164" height="752" alt="image" src="https://github.com/user-attachments/assets/d2dab8e5-ae1b-4db2-b1e7-4672d2914fc0" />

🌐 **https://token.mall199.com**

[![DeepSeek API](https://img.shields.io/badge/DeepSeek-API-blue)](https://token.mall199.com)
[![PayPal](https://img.shields.io/badge/Payment-PayPal-00457C)](https://token.mall199.com)
[![OpenAI Compatible](https://img.shields.io/badge/OpenAI-Compatible-green)](https://token.mall199.com)

---

## 🚀 What is Token Gateway?

**Token Gateway** is a lightweight API proxy that gives international developers access to **DeepSeek's powerful LLM models** — without needing a Chinese phone number, WeChat, or Alipay.

**Pay with PayPal. Start building in minutes.**

---

## ✨ Why Token Gateway?

| Problem | Solution |
|---------|----------|
| ❌ DeepSeek requires Chinese phone number | ✅ **No phone number needed** |
| ❌ Only WeChat/Alipay accepted | ✅ **PayPal payments only** |
| ❌ Complex signup process | ✅ **Sign up & get API key instantly** |
| ❌ Need to rewrite SDK code | ✅ **OpenAI API compatible — drop-in replacement** |

---

## 🔌 OpenAI Compatible

Use any OpenAI SDK. Just change the base URL and API key:

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

Works with **Python, Node.js, Go, curl, LangChain, LlamaIndex** — any OpenAI-compatible client.

---

## 💰 Pricing

| Model | Input (per 1M tokens) | Output (per 1M tokens) |
|-------|----------------------|-----------------------|
| ⚡ **DeepSeek V4 Flash** | $0.50 | $1.00 |
| 🧠 **DeepSeek V4 Pro** | $1.50 | $3.00 |

- 🎯 **$1 starter package** — try before you commit
- 💸 **No subscription**, no monthly fees
- ⏳ **Balance never expires**
- 📊 **Real-time usage dashboard**

---

## 🛠 How It Works

```
1. Sign up → Get your API key
2. Top up balance with PayPal
3. Use any OpenAI SDK with our base URL
4. Done. 🎉
```

---

## 🏗 Tech Stack

- **Backend:** Python (FastAPI)
- **Database:** SQLite
- **Payments:** PayPal REST API
- **Deployment:** VPS + Cloudflare Tunnel

---

## ❓ FAQ

**Q: Do I need a Chinese phone number?**
A: No. Just a PayPal account. That's the whole point.

**Q: Can I use my existing OpenAI code?**
A: Yes. Change `base_url` to `https://token.mall199.com/v1` and your API key. No code changes.

**Q: How do I get my API key?**
A: Instantly after PayPal payment confirmation.

**Q: What if I run out of balance?**
A: API returns 402 error. Top up anytime — no minimum amount.

---

## 🔗 Links

- 🌐 **Website:** https://token.mall199.com
- 📧 **Support:** support@token.mall199.com

---

*Built for developers who need access to great AI models without regional restrictions.*
