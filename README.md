# Tecbeck-Chatbot
🚀 Tecbeck Dual-Agent AI Workflow (n8n)
AI-Powered Client Support + Internal Automation System

A production-grade, fully automated Dual AI Agent System built using n8n, designed for Tecbeck.
This workflow includes:

A Client Support Agent for handling public queries

A Tecbeck Internal Agent for supporting team operations, documentation, and task management

✔ Built for scalability
✔ Production-ready logic
✔ Enterprise workflow structure

🌐 Overview

This workflow uses Google Sheets, Gmail, Google Calendar, and Gemini AI to create a powerful automation system with two intelligent agents:

🔵 Client Agent (Public-Facing)

Helps visitors, leads, and clients by answering queries, collecting requirements, and providing official Tecbeck information.

🟣 Tecbeck Internal Agent

Built exclusively for internal use — assists team members with drafting emails, scheduling meetings, generating documents, and supporting technical tasks.

✨ Key Features
🔵 Client Agent — For Users & Leads

🏢 Service Information Delivery

📥 Lead Capture & Email Notifications to Team

📄 Explain Tecbeck Services Clearly & Professionally

🧩 Smart Service Recommendation System

🧠 Conversation Memory for Natural Chat Experiences

🟣 Internal Agent — For Tecbeck Team

📊 Client & Task Database Management via Google Sheets

✍️ Professional Email Drafting

📆 Google Calendar Meeting Scheduler

🧮 Automation Tools: Calculations, Estimates, Time Tracking

📄 Documentation Helper using Styling Agent

🧪 Technical Assistance: Briefs, SOPs, and Workflows

🛠️ Architecture
User Message  
    ↓  
Chat Trigger  
    ↓  
Keyword Router ───────────────┐  
     ↓                        ↓  
Client Agent            Internal Agent  
     ↓                        ↓  
Google Sheets            Google Sheets  
Gmail                    Gmail  
Google Calendar          Google Calendar  
Gemini AI                Gemini AI  
Styling Layer            Styling Layer  


Clean, modular, and scalable for enterprise usage.

🔐 Prerequisites
Required Accounts

Google Cloud (Gemini)

Gmail

Google Sheets

Google Calendar

n8n instance

Required Credentials

Gemini API Key

Gmail OAuth2

Google Sheets OAuth2

Calendar OAuth2

📂 Setup Guide
1️⃣ Prepare Google Sheets
Client_Inquiries (columns)

Name

Email

Phone

Service Needed

Budget

Message

Notes

Internal_Tasks (columns)

Task ID

Assigned To

Priority

Deadline

Description

Status

2️⃣ Import Workflow into n8n

Go to Workflows → Import

Paste the JSON

Save & activate

3️⃣ Connect Credentials

Update each of these nodes:

Gemini Chat Model

Gmail Send Email

Google Sheets (Read/Write)

Google Calendar

4️⃣ Update Sheet IDs

Insert:

Your Google Sheet Document ID

Sheet names: Client_Inquiries, Internal_Tasks

🚀 Usage Instructions
🎯 Agent Routing Logic
User Keyword	Agent Activated
“internal” / “team”	Tecbeck Internal Agent
Anything else	Client Agent
🔵 Client Agent — Examples

“What services does Tecbeck offer?”

“I want to build an app”

“Can someone contact me for a website project?”

“How much does AI automation cost?”

🟣 Internal Agent — Examples

“Internal: draft an email to a client about the UI/UX update”

“Internal: create a task for the development team”

“Internal: schedule a meeting tomorrow at 2 PM”

“Internal: summarize the project requirements”

🧠 Memory System

500-token rolling memory

Maintains context

Prevents overflow

Ensures stable execution

🧩 Customization Options
Modify Prompts (system behavior)

Client Agent Node → Client instructions

Internal Agent Node → Internal rules

Add More Integrations

HubSpot / Salesforce

Twilio (SMS/WhatsApp)

Stripe (Payments)

Google Docs (Document generation)

Memory Adjustment

Modify:

contextWindowLength: 500

🛡️ Best Practices

Keep Sheets clean and validated

Monitor workflow execution logs

Respect Google API rate limits

Test both agents after changes

Separate internal commands carefully

👤 Author

Abdullah Aqeel
AI Automation Expert • Software Quality Assurance Engineer 📧 abdullahaqeel2011@gmail.com

📄 License

This project is licensed for educational and commercial use.
