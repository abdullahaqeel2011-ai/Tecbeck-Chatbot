# Tecbeck-Chatbot
🚀 Tecbeck-Chatbot

Dual-Agent AI Workflow for Tecbeck (n8n)

A smart, automated workflow designed to handle client inquiries and internal team operations using n8n + Gemini AI + Google Workspace.

🌐 Overview

Uses Gemini AI, Google Sheets, Gmail, Google Calendar, n8n

Includes two intelligent agents:

🔵 Client Agent – For leads & public users

🟣 Internal Agent – For Tecbeck team tasks

✨ Key Features
🔵 Client Agent (Public)

🏢 Provides official Tecbeck service information

📥 Collects leads & sends email alerts

📄 Explains services professionally

🧩 Smart service recommendations

🧠 Maintains conversation memory

🟣 Internal Agent (Team)

📊 Manage client & task data via Google Sheets

✍️ Draft professional emails

📆 Schedule meetings through Google Calendar

🧮 Perform calculations & estimates

📄 Generate documents with styling layer

🧪 Assist with SOPs, briefs & internal workflows

🔐 Prerequisites
📌 Required Accounts

Google Cloud (Gemini)

Gmail

Google Sheets

Google Calendar

n8n instance

📌 Credentials Needed

Gemini API Key

Gmail OAuth2

Google Sheets OAuth2

Google Calendar OAuth2

📂 Setup Guide (Summary)

Prepare Google Sheets

Client_Inquiries: Name, Email, Phone, Service Needed, Budget, Message, Notes

Internal_Tasks: Task ID, Assigned To, Priority, Deadline, Description, Status

Import Workflow

Workflows → Import → Paste JSON

Connect Credentials

Gemini AI Model

Gmail

Google Sheets

Google Calendar

Update Sheet IDs

Google Sheet Document ID

Sheet names

🚀 Usage Instructions
🎯 Routing Logic

Messages with “internal” / “team” → Internal Agent

Everything else → Client Agent

🔵 Client Agent Examples

“What services does Tecbeck offer?”

“I want to build a website or mobile app.”

“Do you offer AI automation?”

🟣 Internal Agent Examples

“Internal: draft an email for the design update.”

“Internal: schedule a meeting tomorrow at 2 PM.”

“Internal: add a development task.”

🧠 Memory System

500-token rolling memory

Smooth conversation flow

Prevents memory overload

🧩 Customization Options

🔧 Modify prompts in Client/Internal agent nodes

🔧 Add integrations (HubSpot, Salesforce, Twilio, Stripe, Google Docs)

🔧 Adjust memory (contextWindowLength: 500)

🛡️ Best Practices

Keep Google Sheets clean

Monitor workflow logs

Follow Google API limits

Test both agents after changes

Keep internal keywords private

📄 License

Licensed for educational and commercial use.

👤 Author

Abdullah Aqeel
AI Automation Expert | Software Quality Assurance Engineer
📧 abdullahaqeel2011@gmail.com
