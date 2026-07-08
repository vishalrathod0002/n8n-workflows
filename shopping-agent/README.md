# 🛒 Shopping Agent

An AI-powered shopping assistant built with **n8n**, **Google Gemini**, **Telegram**, and **SearchAPI**. The workflow helps users find the best product deals by accepting either a product URL or a product name and returning the top shopping results.

---

## ✨ Features

- 🔗 Accepts both **product URLs** and **product name searches**
- 🌐 Extracts product information from supported e-commerce pages
- 🔍 Searches Google Shopping for matching products
- 🤖 Uses Google Gemini AI to analyze and rank the best deals
- 💰 Returns the **Top 5 best deals**
- ⭐ Includes price, seller, rating, and direct purchase links
- 📲 Sends results directly to Telegram

---

## 🏗️ Workflow Overview

```
Telegram Trigger
       │
       ▼
Check Input Type
       │
 ┌─────┴────────┐
 │              │
 │ Product URL  │ Product Name
 │              │
 ▼              ▼
Fetch Product   Search Google Shopping
Page                 │
 │                    │
 ▼                    │
Extract Product Info  │
 │                    │
 └──────────┬─────────┘
            ▼
      Merge Results
            │
            ▼
   Check Results Found
            │
      ┌─────┴─────┐
      │           │
      ▼           ▼
 Analyze Deals   No Results
      │
      ▼
Send Telegram Message
```

---

## 🛠️ Technologies Used

- n8n
- Google Gemini 2.5 Flash
- Telegram Bot API
- SearchAPI (Google Shopping)
- HTTP Request Node
- HTML Extraction Node

---

## 📥 Input

The bot accepts two types of input via Telegram.

### Option 1: Product URL

Example:

```
https://www.amazon.in/dp/B0D1234567
```

The workflow will:

- Fetch the webpage
- Extract the product name
- Search Google Shopping
- Return the best deals

---

### Option 2: Product Name

Example:

```
Samsung Galaxy S25 Ultra
```

The workflow searches Google Shopping directly and returns matching products.

---

## 📤 Output

The bot returns the **Top 5 shopping deals**, including:

- 🛍️ Product Name
- 💰 Price
- 🏪 Store
- ⭐ Rating (if available)
- 🔗 Direct product link

Example:

```
🔥 Top 5 Deals for Samsung Galaxy S25 Ultra

🥇 Samsung Galaxy S25 Ultra 256GB

💰 ₹99,999
🏪 Amazon
⭐ 4.8

🔗 https://...

🥈 ...

💡 Tip: Compare prices before purchasing.
```

---

## 🔑 Required Credentials

Before running this workflow, configure the following credentials in n8n:

| Service | Required |
|----------|----------|
| Telegram Bot | ✅ |
| Google Gemini API | ✅ |
| SearchAPI Key | ✅ |

---

## 📦 Installation

1. Clone this repository.

```bash
git clone https://github.com/<your-username>/n8n-workflows.git
```

2. Open n8n.

3. Navigate to:

```
shopping-agent/
```

4. Import:

```
shopping-agent.json
```

5. Configure all required credentials.

6. Activate the workflow.

---

## ⚙️ Workflow Logic

1. User sends a product URL or product name to the Telegram bot.
2. The workflow detects the input type.
3. If a URL is provided, it extracts the product details from the webpage.
4. Google Shopping is queried using SearchAPI.
5. Google Gemini analyzes the shopping results.
6. The AI filters irrelevant listings and ranks the best deals.
7. The formatted response is sent back to the user on Telegram.

---

## 📂 Project Structure

```
shopping-agent/
├── README.md
├── shopping-agent.json
├── architecture.png
└── .env.example
```

---

## 🚀 Future Improvements

- Amazon affiliate links
- Multi-country shopping support
- Price history tracking
- Product comparison
- Wishlist support
- Price drop notifications
- Multi-language support

---

## 📄 License

This project is licensed under the MIT License.

---

## ⭐ Support

If you found this workflow useful, consider giving this repository a ⭐ on GitHub.