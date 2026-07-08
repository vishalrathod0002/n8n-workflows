# 🌤️ Weather Reports

An automated weather reporting workflow built with **n8n**, **OpenWeatherMap API**, and **Telegram**. The workflow fetches the latest weather information for a configured city every **2 hours** and delivers a formatted weather report directly to a Telegram chat.

---

## ✨ Features

- ⏰ Automatically runs every **2 hours**
- 🌍 Fetches real-time weather data using the OpenWeatherMap API
- 🌡️ Reports current temperature and "feels like" temperature
- 💨 Displays humidity, pressure, wind speed, cloud cover, and visibility
- 📲 Sends beautifully formatted weather reports to Telegram
- ⚠️ Sends an error notification if the weather API request fails

---

## 🏗️ Workflow Overview

```text
Schedule Trigger (Every 2 Hours)
                │
                ▼
      Set Configuration
                │
                ▼
     Fetch Weather Data
                │
      ┌─────────┴─────────┐
      │                   │
      ▼                   ▼
Format Weather Data   Error Alert
      │
      ▼
Send Telegram Report
```

---

## 🛠️ Technologies Used

- n8n
- OpenWeatherMap API
- Telegram Bot API
- HTTP Request Node
- Set Node
- Schedule Trigger

---

## 📥 Configuration

Before running the workflow, configure the following values:

| Parameter | Description |
|-----------|-------------|
| City | City to monitor (e.g., Pune, London, New York) |
| OpenWeatherMap API Key | Your API key from OpenWeatherMap |
| Telegram Bot | Telegram Bot credentials in n8n |
| Chat ID | Telegram chat ID where reports will be sent |

---

## 📤 Sample Weather Report

```text
🌤 Weather Report
━━━━━━━━━━━━━━━

📍 Location
🏙 Pune, IN

🌡 Temperature
🌡️ Current: 29°C
🤒 Feels Like: 31°C
☁️ Conditions: Broken Clouds

💨 Atmospheric Data
📊 Pressure: 1012 hPa
💧 Humidity: 74%
🌬 Wind Speed: 4.2 m/s
☁️ Cloud Cover: 60%
👁 Visibility: 10 km

🕐 Updated: Jul 8, 2026 10:00 AM
```

---

## 🔑 Required Credentials

| Service | Required |
|----------|----------|
| Telegram Bot | ✅ |
| OpenWeatherMap API | ✅ |

---

## 📦 Installation

1. Clone this repository.

```bash
git clone https://github.com/<your-username>/n8n-workflows.git
```

2. Open **n8n**.

3. Navigate to:

```
weather-reports/
```

4. Import:

```
weather-reports.json
```

5. Configure the following:
   - OpenWeatherMap API Key
   - City Name
   - Telegram Bot Credentials
   - Telegram Chat ID

6. Activate the workflow.

---

## ⚙️ Workflow Logic

1. The workflow is triggered automatically every **2 hours**.
2. Configuration values (city and API key) are loaded.
3. Weather data is fetched from the OpenWeatherMap API.
4. The response is formatted into a user-friendly weather report.
5. The report is sent to the configured Telegram chat.
6. If the API request fails, an error notification is sent instead.

---

## 📂 Project Structure

```text
weather-reports/
├── README.md
├── weather-reports.json
├── architecture.png
└── .env.example
```

---

## 🚀 Future Improvements

- 🌦 5-day weather forecast
- 🌍 Support for multiple cities
- 🌅 Sunrise and sunset information
- 🌧 Rain and storm alerts
- 📊 Weather history logging
- 📧 Email notifications
- 📱 Slack and Discord integration
- 🤖 AI-generated weather summaries

---

## 📄 License

This project is licensed under the MIT License.

---

## ⭐ Support

If you found this workflow useful, consider giving this repository a ⭐ on GitHub.