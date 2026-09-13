# Smart-email-triage-gemini-n8n

**Overview:**

This repository contains a production-ready Email Automation Workflow built with n8n and Google Gemini 1.5 Flash. The system automates incoming email triage by parsing subjects and body content, categorizing customer queries, determining priority levels, logging structured data into Google Sheets, and automatically creating formal response drafts in Gmail.


<img width="953" height="486" alt="N8N Canvas" src="https://github.com/user-attachments/assets/40b93d72-30d8-449a-a0c7-b7719059219c" />


**Key Features:**

1. Automated Email Ingestion: Triggers instantly upon receiving a new email via Gmail API.

2. Intelligent AI Categorization: Classifies emails into categories (e.g., Late Delivery, Broken Product, Order Cancellation, General Query).

3. Priority Escalation: Automatically assigns Urgent, Medium, or Low priority based on the category.

4. Structured Data Extraction: Enforces JSON-only output from Gemini 1.5 Flash using custom prompt rules and a JavaScript parsing node.

5. Database Logging: Appends processed metadata directly into Google Sheets for record-keeping.

<img width="959" height="440" alt="Excel sheet preview" src="https://github.com/user-attachments/assets/72d32920-21cc-48f4-8af0-0459d41a7072" />


6. Formal Draft Generation: Crafts polite, professional English draft responses directly inside Gmail for human review before sending.

a. Customer Email:
<img width="911" height="457" alt="Customer Query" src="https://github.com/user-attachments/assets/b670c990-3e9f-4704-828f-d0c4d73a73bc" />


b. AI Draft Reply:
<img width="916" height="425" alt="Ai Generated Draft" src="https://github.com/user-attachments/assets/70e10581-bdc4-4eb0-b456-e5bd60001f30" />



**Tech Stack:**

Orchestration: n8n Workflow Engine

AI Model: Google Gemini 3.6 Flash (via Google AI Studio)

Integrations: Gmail API, Google Sheets API

Data Processing: JavaScript (n8n Code Node)

**Setup & Usage:**

Import the workflow.json file into your n8n instance.

Authenticate your Google AI Studio API Key and Gmail OAuth2 credentials.

Configure the Google Sheets node to match your spreadsheet structure.

Activate the workflow
