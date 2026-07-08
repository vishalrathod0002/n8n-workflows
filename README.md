# 🚀 n8n Workflows Collection

A centralized collection of reusable, production-ready **n8n workflows** for AI agents, automation, API integrations, and business processes.

Each workflow is self-contained and includes:
- 📄 Workflow documentation (`README.md`)
- 🔄 Exported n8n workflow (`.json`)
- 🖼️ Workflow architecture/screenshot (optional)
- ⚙️ Environment variable example (if required)

---

## 📂 Repository Structure

```text
n8n-workflows/
│
├── README.md
├── LICENSE
├── .gitignore
│
├── shopping-agent/
│   ├── README.md
│   ├── shopping-agent.json
│   ├── architecture.png
│   └── .env.example
│
├── send-email-agent/
│   ├── README.md
│   ├── send-email-agent.json
│   ├── architecture.png
│   └── .env.example
│
├── github-monitor/
│   ├── README.md
│   ├── github-monitor.json
│   └── architecture.png
│
├── rag-agent/
│   ├── README.md
│   ├── rag-agent.json
│   └── architecture.png
│
└── shared/
    ├── setup.md
    └── credentials.md
```

---

## 📋 Available Workflows

| Workflow | Description | Status |
|----------|-------------|--------|
| 🛒 Shopping Agent | AI-powered shopping assistant | ✅ |
| 📧 Send Email Agent | Automates email generation and delivery | ✅ |
| 🐙 GitHub Monitor | Monitors GitHub repositories and events | ✅ |
| 🤖 RAG Agent | AI-powered Retrieval-Augmented Generation workflow | ✅ |

> Each workflow has its own documentation with setup instructions, required credentials, and usage examples.

---

## 🚀 Getting Started

1. Clone this repository.

```bash
git clone https://github.com/<your-username>/n8n-workflows.git
```

2. Open **n8n**.

3. Navigate to the workflow you want to use.

4. Import the corresponding `.json` file into n8n.

5. Configure the required credentials.

6. Execute or activate the workflow.

---

## 📖 Documentation

Each workflow contains its own `README.md` with:
- Overview
- Features
- Prerequisites
- Installation
- Required credentials
- Workflow explanation
- Inputs and outputs
- Customization options

Shared documentation is available in the `shared/` directory.

---

## 🔑 Credentials

Some workflows require external services such as:

- OpenAI
- Google Gmail
- GitHub
- Slack
- Discord
- PostgreSQL
- Pinecone
- Supabase
- Other third-party APIs

Refer to each workflow's documentation for the required credentials.

---

## 🤝 Contributing

Contributions are welcome!

To add a new workflow:

1. Create a new folder under the repository.
2. Add the exported workflow (`.json`).
3. Include a `README.md` explaining the workflow.
4. Add an architecture image or screenshot (optional).
5. Include a `.env.example` file if environment variables are required.
6. Submit a pull request.

---

## 📜 License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

## ⭐ Support

If you find these workflows useful, consider giving this repository a ⭐ on GitHub.
