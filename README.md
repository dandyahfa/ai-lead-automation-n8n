# 🚀 AI-Powered Lead Prioritization & Instant Notification System

An automated end-to-end workflow built using **n8n**, **Google Gemini AI**, **Slack**, and **Google Sheets (via Google Apps Script)** to automatically capture, analyze, sort, and store incoming website leads in real-time.

---

## 🏗️ Architecture & Workflow Overview
1. **Webhook Node:** Captures incoming lead data (Name, Company, Message, Budget) via HTTP POST requests from the website form.
2. **AI Agent (Google Gemini):** Analyzes the lead's message and budget context, determining urgency, intent, and priority level (`High`, `Medium`, `Low`) while generating targeted sales recommendations.
3. **Google Apps Script & Google Sheets:** Automatically parses the structured AI output and logs the lead details into a centralized database spreadsheet in real-time.
4. **Slack Integration:** Triggers conditional routing to instantly push high-priority alerts to dedicated Slack channels, allowing the sales team to follow up within minutes.

---

## 🛠️ Tech Stack
* **Workflow Automation:** n8n
* **Artificial Intelligence:** Google Gemini API (LLM)
* **Database & Backend:** Google Sheets, Google Apps Script (Web App API)
* **Communication:** Slack API

---

## 📂 Project Structure
- `index.html` — Frontend contact form UI for capturing lead data.
- `script.js` — JavaScript logic handling asynchronous form submission via Fetch API to the n8n webhook.
- **n8n Workflow Schema:** Handles data ingestion, AI processing, conditional logic, and external API requests.
- **Google Apps Script (`doPost`):** Backend script for appending structured lead data directly into Google Sheets.

---

## 💡 Key Benefits
* **Zero-Lag Lead Qualification:** Eliminates manual data sorting by letting AI evaluate potential clients instantly.
* **Cost-Effective Backend:** Uses lightweight Google Apps Script Web Apps for fast database logging.
* **Real-Time Team Alignment:** Ensures high-value prospects never slip through the cracks by triggering instant Slack notifications.
