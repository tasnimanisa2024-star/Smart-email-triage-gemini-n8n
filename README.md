# Smart-email-triage-gemini-n8n

**Overview:**

This repository contains a production-ready Email Automation Workflow built with n8n and Google Gemini 1.5 Flash. The system automates incoming email triage by parsing subjects and body content, categorizing customer queries, determining priority levels, logging structured data into Google Sheets, and automatically creating formal response drafts in Gmail.

**Key Features:**

Automated Email Ingestion: Triggers instantly upon receiving a new email via Gmail API.

Intelligent AI Categorization: Classifies emails into categories (e.g., Late Delivery, Broken Product, Order Cancellation, General Query).

Priority Escalation: Automatically assigns Urgent, Medium, or Low priority based on the category.

Structured Data Extraction: Enforces JSON-only output from Gemini 1.5 Flash using custom prompt rules and a JavaScript parsing node.

Database Logging: Appends processed metadata directly into Google Sheets for record-keeping.

Formal Draft Generation: Crafts polite, professional English draft responses directly inside Gmail for human review before sending.

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
