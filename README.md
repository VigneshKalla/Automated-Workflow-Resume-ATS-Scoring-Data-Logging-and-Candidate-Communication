# 🚀  Automated-Workflow-Resume-ATS-Scoring-Data-Logging-and-Candidate-Communication

An end-to-end automation system built using **n8n** to streamline resume intake, ATS scoring, candidate triaging, and email communication.
This workflow eliminates repetitive HR tasks and reduces manual screening efforts by **up to 80%**, making it ideal for HR teams, staffing agencies, and automated hiring systems.

---

## 📌 Overview

This project automates the complete hiring pipeline—from collecting resumes submitted via Telegram to scoring them through ATS logic and notifying candidates with personalized emails.

The workflow ensures:

✔ Faster candidate screening
✔ 100% automated triage
✔ Consistent communication
✔ Cleaner data storage and tracking

---

## 🧩 Features Breakdown

### **1️⃣ Resume Intake via Telegram Bot**

Candidates can upload:

* A **single PDF**, or
* A **ZIP file** containing one PDF

Your n8n Telegram Trigger Node captures the file automatically and passes it to the next stage for processing.

---

### **2️⃣ Intelligent File Processing & ATS Scoring**

The workflow:

* Detects if the uploaded file is PDF or ZIP
* Extracts PDFs from ZIP files
* Sends the resume to **Google Gemini / LLM model** for ATS evaluation
* Receives a clean, structured ATS score output

This enables accurate and automated filtering of candidate profiles.

---

### **3️⃣ Automated Decision Routing**

Based on the returned ATS score:

**✔ Higher or valid score → “Accepted Candidates” Google Sheet**
**✖ Lower or invalid score → “Rejected Candidates” Google Sheet**

No manual screening required — the workflow makes real-time decisions.

---

### **4️⃣ Fully Automated Candidate Email Communication**

Depending on the triage result:

* **Accepted Candidates** receive a personalized acceptance email with next steps.
* **Rejected Candidates** receive a polite, professional rejection email.

This ensures quick, consistent, and human-like communication—without manual intervention.

---

## 💡 Key Highlights

* ⚡ **80% reduction** in manual resume screening time
* 🤖 Full automation — no human involvement required after setup
* 🧠 Smart ATS scoring using LLM-based analysis
* 📊 Clean segregation of accepted vs. rejected candidates
* 📥 Unified workflow from *resume intake → scoring → routing → emailing*
* 🛠️ Perfect example of a low-code automation pipeline using **n8n**

---

## 🛠️ Tech Stack

| Component               | Usage                        |
| ----------------------- | ---------------------------- |
| **n8n**                 | Core automation engine       |
| **Telegram Bot**        | Candidate resume submissions |
| **Google Gemini (LLM)** | ATS scoring & text analysis  |
| **Google Sheets**       | Candidate data storage       |
| **Email Node**          | Automated communication      |

---

## 📂 Workflow Architecture

```
Telegram Bot → File Processing → ATS Scoring → Conditional Score Check
     → Google Sheet (Accepted/Rejected) → Automated Email Notification
```

---

## 📸 Screenshots (Add When Available)

* Telegram Bot submission
* n8n workflow screenshot
* Google Sheet entries
* Email templates


---

## 📘 How to Use

1. Clone this repository
2. Import the workflow JSON into **n8n**
3. Configure your credentials for:

   * Telegram Bot
   * Google Sheets
   * Google Gemini (or your LLM provider)
   * Email service (SMTP / Gmail API)
4. Deploy and activate the workflow
5. Share your Telegram bot link with candidates

---

## ✨ Future Enhancements

* Resume parsing with structured output
* Skills extraction & matching with job descriptions
* Multi-job role support
* Candidate scoring dashboards
* Automated interview scheduling

---

## 🙌 Contributing

Contributions are welcome!
Feel free to submit issues or open pull requests to improve the workflow.

---
