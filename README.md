# 🚀 n8n Workflows Collection

A curated collection of production-ready **n8n workflows** for AI automation, integrations, notifications, and productivity.

Each workflow is self-contained and includes:
- 📄 Documentation (`README.md`)
- 🔄 Exported n8n workflow (`.json`)
- 🖼️ Workflow architecture (optional)
- ⚙️ Environment configuration example (if required)

---

# 📂 Repository Structure

```text
n8n-workflows/
│
├── ai-email-assistant/
├── shopping-agent/
├── webhook-to-telegram-notification/
└── weather-reports-agent/
```

---

# 📋 Available Workflows

| Workflow | Description | Technologies |
|----------|-------------|--------------|
| 📧 AI Email Assistant | Generate and send professional emails using AI and Gmail. | OpenAI, Gmail, n8n |
| 🛒 Shopping Agent | Find the best shopping deals from a product link or product name using AI. | Google Gemini, SearchAPI, Telegram |
| 📩 Webhook to Telegram Notification | Receive HTTP webhook requests and instantly forward them to Telegram. | Webhook, Telegram |
| 🌤 Weather Reports Agent | Fetch weather information every 2 hours and send reports to Telegram. | OpenWeatherMap, Telegram |

---

# 🚀 Getting Started

## 1. Clone the Repository

```bash
git clone https://github.com/<your-username>/n8n-workflows.git
```

## 2. Open n8n

Launch your local or hosted n8n instance.

## 3. Import a Workflow

Navigate to the desired workflow folder and import the corresponding `.json` file into n8n.

## 4. Configure Credentials

Depending on the workflow, configure the required credentials in n8n.

Examples include:

- OpenAI
- Google Gemini
- Gmail OAuth2
- Telegram Bot
- OpenWeatherMap API
- SearchAPI

## 5. Activate the Workflow

Save and activate the workflow to start using it.

---

# 🛠 Technologies Used

- n8n
- OpenAI GPT
- Google Gemini
- Gmail API
- Telegram Bot API
- OpenWeatherMap API
- SearchAPI
- HTTP Requests
- Webhooks

---

# 📂 Workflow Details

## 📧 AI Email Assistant

Generate professional emails from natural language prompts using AI and send them through Gmail.

**Highlights**
- AI-generated email content
- Gmail integration
- Conversation memory
- Professional formatting

---

## 🛒 Shopping Agent

Searches Google Shopping using either a product URL or product name and returns the top deals ranked by AI.

**Highlights**
- Product URL support
- Product name search
- AI deal analysis
- Telegram notifications

---

## 📩 Webhook to Telegram Notification

Receives HTTP POST requests and forwards the payload as a formatted Telegram message.

**Highlights**
- Webhook endpoint
- Instant Telegram notifications
- Lightweight integration
- Easy API connectivity

---

## 🌤 Weather Reports Agent

Automatically retrieves weather information every two hours and sends a detailed report to Telegram.

**Highlights**
- Scheduled execution
- Real-time weather data
- Error notifications
- Telegram delivery

---

# 📦 Requirements

Some workflows require one or more of the following services:

- OpenAI API
- Google Gemini API
- Gmail OAuth2
- Telegram Bot API
- OpenWeatherMap API
- SearchAPI

Refer to each workflow's **README.md** for setup instructions and required credentials.

---

# 🤝 Contributing

Contributions are welcome!

To add a new workflow:

1. Create a new folder.
2. Add the exported workflow (`.json`).
3. Include a detailed `README.md`.
4. Add an architecture image or screenshot (optional).
5. Include a `.env.example` file if environment variables are required.
6. Submit a Pull Request.

---

# 📄 License

This repository is licensed under the **MIT License**.

---

# ⭐ Support

If you find these workflows useful:

- ⭐ Star this repository
- 🍴 Fork it
- 🛠 Contribute new workflows
- 💡 Share your ideas and improvements

Happy Automating! 🚀