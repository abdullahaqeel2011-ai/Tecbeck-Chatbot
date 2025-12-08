# Tecbeck-Chatbot
🚀 Tecbeck-Chatbot

A powerful Dual-Agent AI Workflow built using n8n for Tecbeck — designed to handle both client-facing conversations and internal team operations with accuracy, professionalism, and automation efficiency.

🌐 Overview

This workflow combines the power of Google Sheets, Gmail, Google Calendar, and Gemini AI to deliver two intelligent agents:

🔵 Client Agent (Public-Facing)

Helps visitors, leads, and clients by answering queries, gathering requirements, and sharing official Tecbeck information.

🟣 Internal Agent (Tecbeck Team)

Supports team tasks such as email drafting, documentation, meeting scheduling, and internal operations.

✨ Key Features
🔵 Client Agent — For Users & Leads

🏢 Provides accurate Tecbeck service information

📥 Captures leads and sends email notifications to the team

📄 Delivers professional explanations of services

🧩 Smart service recommendations

🧠 Conversation memory for natural and smooth interactions

🟣 Internal Agent — For Tecbeck Team

📊 Manage client/task data through Google Sheets

✍️ Draft professional emails

📆 Schedule meetings using Google Calendar

🧮 Perform calculations, estimates, and internal utilities

📄 Help generate documents using the styling layer

🧪 Assist with SOPs, briefs, internal workflows

🔐 Prerequisites
📌 Required Accounts

Google Cloud (Gemini AI)

Gmail

Google Sheets

Google Calendar

n8n instance

📌 Required Credentials

Gemini API Key

Gmail OAuth2

Google Sheets OAuth2

Google Calendar OAuth2

📂 Setup Guide
1️⃣ Prepare Google Sheets

Client_Inquiries columns:

Name

Email

Phone

Service Needed

Budget

Message

Notes

Internal_Tasks columns:

Task ID

Assigned To

Priority

Deadline

Description

Status

2️⃣ Import Workflow

Go to Workflows → Import

Paste the JSON

Save & activate

3️⃣ Connect Credentials

Update these nodes with your credentials:

Gemini AI Model

Gmail Send Email

Google Sheets (Read/Write)

Google Calendar

4️⃣ Update Sheet IDs

Add your:

Google Sheet Document ID

Sheet names: Client_Inquiries, Internal_Tasks

🚀 Usage Instructions
🎯 Agent Routing Logic
User Keyword	Agent Used
“internal” / “team”	Tecbeck Internal Agent
Anything else	Client Agent
🔵 Client Agent — Example Prompts

“What services does Tecbeck offer?”

“I want to build a website/mobile app.”

“Can someone from Tecbeck contact me?”

“Do you offer AI automation?”

🟣 Internal Agent — Example Prompts

“Internal: draft an email for the design update.”

“Internal: add a task for the developer.”

“Internal: schedule a meeting tomorrow at 2 PM.”

“Internal: summarize the project requirements.”

🧠 Memory System

500-token rolling memory

Maintains smooth conversation flow

Prevents overload

Ensures consistent performance

🧩 Customization Options
🔧 Modify Prompts

Update system messages in the Client Agent or Internal Agent nodes.

🔧 Add Integrations

HubSpot / Salesforce

Twilio (SMS/WhatsApp)

Stripe (Payments)

Google Docs (Reports, proposals)

🔧 Adjust Memory

Modify:

contextWindowLength: 500

🛡️ Best Practices

Ensure Google Sheets have clean and consistent data

Monitor workflow logs for errors

Follow Google API quota limits

Test both agents before production

Keep internal commands separate from public use

📄 License

This project is licensed for educational and commercial use.

👤 Author

Abdullah Aqeel 

📧 abdullahaqeel2011@gmail.com

AI Automation Expert | Software Quality Assurance Engineer 

📄 License

This project is licensed for educational and commercial use.
