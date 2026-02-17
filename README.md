# AI Email Processing & Document Intelligence Automation

End-to-end automation built with **n8n** that processes incoming Gmail emails, extracts document text using OCR, analyzes content with AI and automatically stores structured results in Google Sheets and Google Drive.

This system eliminates manual document processing and enables scalable intelligent automation workflows.

---

## Workflow Overview

This automation monitors Gmail inboxes, detects attachments, extracts structured data and logs the results automatically.

### Process Flow

Gmail Trigger  
→ Retrieve Email Data  
→ Preprocess Email  
→ Classify Email Type  

If attachment is supported (PDF / Image):

→ OCR Text Extraction  
→ AI Content Analysis  
→ Structured Data Processing  
→ Save Original File to Google Drive  
→ Register Structured Data in Google Sheets  

If attachment unsupported:

→ Store file in Google Drive  
→ Register for manual review  

If document processing fails:

→ Register error in Google Sheets  

---

## Workflow Diagram

![Workflow Diagram](./assets/aiEmailProcessing.jpg)

---

## Features

• Automated Gmail monitoring  
• OCR document text extraction  
• AI-powered content analysis  
• Automatic invoice data extraction  
• Google Drive file storage  
• Google Sheets structured logging  
• Error handling and fallback routing  
• Fully automated document processing pipeline  

---

## Tech Stack

Automation Platform:

• n8n  

Integrations:

• Gmail API  
• Google Drive API  
• Google Sheets API  

Processing:

• OCR Space API  
• Generative AI  
• JavaScript  

---

## Extracted Data Fields

The system automatically extracts:

• Issue Date  
• Client / Provider  
• Invoice Number  
• Tax values  
• Total amount  
• Currency  
• Payment status  
• Processing timestamp  

---

## Setup Instructions

Import workflow into n8n:

1. Open n8n
2. Click Import Workflow
3. Select ai-email-document-intelligence-n8n.json

Configure credentials:

• Gmail account  
• Google Drive account  
• Google Sheets account  
• OCR API Key  
• AI API Key  

Replace placeholders:

REPLACE_WITH_YOUR_SHEET_URL  
REPLACE_WITH_RESOURCE_ID  

Activate workflow.

---

## Use Cases

Invoice automation  
Accounting automation  
Document intake automation  
Business process automation  
Document intelligence pipelines  

---

## Author

Maria Fernanda Moreno

Automation Developer  
AI Automation Specialist  
n8n Developer  

## Proyectos

Live Portfolio:

showcase-de-automatizaciones-y-webs.vercel.app
---