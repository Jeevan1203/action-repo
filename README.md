# 🚀 Action Repo (TechStaX Assignment)

This is the companion repository used to trigger GitHub webhook events for the main [Webhook Dashboard](https://github.com/Jeevan1203/webhook-repo) project.

---

## 🧪 Purpose

This repo is used to:

- Trigger `push` events by committing code
- Trigger `pull_request` events by opening PRs
- Trigger `merge` events by merging PRs (via GitHub UI)

These events are sent via webhook to the Flask app in the [webhook-repo](https://github.com/Jeevan1203/webhook-repo), which stores them in MongoDB and displays them on a live dashboard.

---

## 🔧 How It Works

This repo is connected via GitHub Webhook to the Flask backend.

Webhook Settings:
- Payload URL: `https://<your-ngrok-url>/webhook`
- Content type: `application/json`
- Events: ✅ Push, ✅ Pull Request, ✅ Merge

---

## 📂 Typical Activity

Example event triggers:
- Push new commits to `main`
- Create a new branch and open a pull request
- Merge a PR via GitHub UI

All of the above will be logged and displayed in the dashboard UI.

---

## 📁 Files (Optional)

You can include any dummy files:
- `main.py` — simple script
- `README.md` — this file
- Any file to help generate meaningful commits

---

## 🙌 Author

**Jeevan Kumar Adapa**  
Built for TechStaX Developer Assessment 2025
