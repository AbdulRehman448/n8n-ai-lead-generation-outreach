# 🤖 AI Lead Generation & Outreach Bot — n8n

Automated cold outreach pipeline that reads leads, generates personalized emails using Gemini AI, sends via Gmail, and tracks status in Google Sheets.

## 🚀 What It Does

- 📋 Reads leads from Google Sheets (name, company, role, industry, pain point)
- 🧠 Generates personalized cold emails using **Gemini AI**
- 📧 Sends emails automatically via Gmail
- 📊 Saves generated messages to Outreach sheet
- ✅ Marks leads as Sent with timestamp
- 🔄 Skips already contacted leads automatically

## 🏗️ Workflow

Manual Trigger → Read Leads → Filter Valid Leads →
Generate Message (Gemini) → Prepare Data →
Save to Sheet → Send Email → Mark as Sent

## 🛠️ Tech Stack

| Tool | Usage |
|------|-------|
| n8n Cloud | Workflow orchestration |
| Google Gemini AI | Personalized email generation |
| Google Sheets | Lead storage and tracking |
| Gmail OAuth2 | Email dispatch |

## ⚙️ Setup

1. Import `workflow.json` into n8n Cloud
2. Connect Google Sheets OAuth2 credentials
3. Connect Gmail OAuth2 credentials
4. Add Gemini API key
5. Update Spreadsheet ID in Google Sheets nodes
6. Add leads to the Leads tab
7. Run manually

## 📋 Google Sheets Structure

**Leads tab columns:**
`name | company | role | email | industry | pain_point`

**Outreach tab columns:**
`name | company | email | generated_message | status | sent_at`

## 📬 Contact

**Abdul Rehman Ali**  
[LinkedIn](https://www.linkedin.com/in/abdul-rehman-ali/) | [Portfolio](https://abdulrehmanali.netlify.app/) | abdulrehman.tp.786@gmail.com
