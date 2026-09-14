# AI Car Dealership Lead Generation & Chatbot

An AI-powered automation system for a car dealership built with **n8n**.

The system automates the lead collection process, stores customer requests, notifies the sales employee, and gives the customer access to an AI chatbot trained on the dealership's data.

## 🚗 Project Overview

The project is designed for a car dealership that receives customer requests through an online form.

After the customer submits the form, the automation processes the information, stores it in Google Sheets, and sends automated emails to both the customer and the dealership employee.

The customer email also contains a link to an AI chatbot that can answer questions about the dealership and available cars.

## 🔄 Workflow

```text
Customer
   │
   ▼
Lead Form
   │
   ▼
Data Processing
   │
   ▼
Google Sheets
   │
   ├──────────────► Customer Email
   │                    │
   │                    ▼
   │              Chatbot Link
   │                    │
   │                    ▼
   │              AI Car Chatbot
   │
   └──────────────► Employee Email
                        │
                        ▼
                   New Lead Alert
📋 Lead Form

The customer fills out a form with information such as:

Name
Phone Number
Email
Request Type
Preferred Car Type
Budget
Notes
Preferred Contact Time

The submitted information is processed before being stored.

📊 Google Sheets

After processing the form data, the lead is automatically stored in Google Sheets.

This allows the dealership employee to easily track and manage customer requests.

Example:

Name	Phone	Email	Car Type	Budget	Request
Ahmed	010xxxxxxx	ahmed@email.com	Sedan	1,200,000 EGP	Buy
📧 Automated Customer Email

After the lead is successfully submitted, the customer automatically receives an email confirming that their request has been received.

The email also contains a link to the dealership's AI chatbot.

Example:

Thank you for contacting us. We have received your request successfully.

You can also chat with our AI assistant to ask about available cars, prices, specifications, and other dealership information.

👨‍💼 Employee Notification

The dealership employee automatically receives an email whenever a new customer request is submitted.

The notification contains the customer's lead information so the sales team can follow up.

🤖 AI Car Dealership Chatbot

The project includes an AI chatbot that customers can access from the confirmation email.

The chatbot is connected to the dealership's data/knowledge base and can answer questions about:

Available cars
Car models
Prices
Specifications
Features
Dealership information

The chatbot is designed to provide customers with quick answers without requiring a sales employee to answer every basic question manually.

🧠 AI & Knowledge Base

The chatbot uses the dealership's data as its knowledge source.

This allows the chatbot to provide answers based on the dealership's actual information instead of relying only on general AI knowledge.

The system can be extended using RAG (Retrieval-Augmented Generation) to retrieve relevant information from the dealership's knowledge base before generating an answer.

🛠️ Technologies
n8n — Workflow automation
Google Sheets — Lead storage
Gmail — Automated email notifications
AI Agent — Intelligent lead/chat handling
LLM — Natural language understanding and generation
RAG / Knowledge Base — Dealership information
JavaScript — Data processing
✨ Features
Lead generation form
Automated data processing
Google Sheets integration
Automatic customer confirmation
Automatic employee notification
AI-powered dealership chatbot
Dealership-specific knowledge base
Automated customer support
Scalable sales automation workflow
📁 Repository Structure
ai-lead-chatbot/
│
├── README.md
├── workflow.json
└── screenshot.png
🔐 Security

Do not upload:

API keys
Passwords
Access tokens
Private credentials
Customer personal data

Before uploading the n8n workflow to GitHub, make sure all sensitive credentials have been removed.

🎯 Project Goal

The main goal of this project is to automate the first stage of the car dealership sales process.

Instead of manually collecting customer information, notifying employees, and answering basic questions, the system handles these tasks automatically.

This helps the dealership:

Save time
Reduce manual work
Organize leads
Respond to customers faster
Provide 24/7 basic customer support
Improve the overall sales workflow

**اسم الـ repo:** `ai-lead-chatbot` مناسب جدًا للمشروع ده.
create a good readme file 

Absolutely. Here’s a professional GitHub-ready README.md for your car dealership n8n project, written to look like a real portfolio project without overclaiming.

# 🚗 AI Car Dealership Lead Generation & Chatbot

An AI-powered automation workflow built with **n8n** for a car dealership.

The system automates the process of collecting customer inquiries, processing and storing lead information, notifying the dealership team, and providing customers with access to an AI chatbot that can answer questions based on the dealership's knowledge base.

---

## 📌 Project Overview

The goal of this project is to automate the customer lead process from the first form submission until the customer starts interacting with the dealership's AI chatbot.

Instead of handling every lead manually, the workflow automatically:

1. Collects customer information through a form.
2. Processes and organizes the submitted data.
3. Stores the lead in **Google Sheets**.
4. Sends a confirmation email to the customer.
5. Sends a notification email to the dealership employee.
6. Provides the customer with a link to the AI chatbot.
7. Allows the customer to ask questions about the dealership and available services/cars.

---

## 🔄 Workflow

```text
Customer
   │
   ▼
📝 Lead Form
   │
   ▼
⚙️ Data Processing
   │
   ├──────────────► 📊 Google Sheets
   │
   ├──────────────► 📧 Customer Confirmation Email
   │                         │
   │                         ▼
   │                    🤖 AI Chatbot
   │
   └──────────────► 📧 Employee Notification
✨ Features
📝 Lead Collection

Customers submit their information through an online form.

Example information:

Name
Email
Phone Number
Car preferences
Budget
Customer request
Additional notes
⚙️ Automated Data Processing

The workflow processes the submitted information before storing it.

This helps keep lead data organized and ready for the dealership team.

📊 Google Sheets Integration

Every new lead is automatically added to a Google Sheet.

This provides the dealership with a simple way to:

View new leads
Track customer requests
Organize customer information
Follow up with potential customers
📧 Automated Customer Email

After submitting the form, the customer automatically receives a confirmation email.

The email confirms that the request has been received and provides a link to the dealership's AI chatbot.

🔔 Employee Notification

The dealership employee receives an automated notification when a new customer submits a request.

This allows the team to respond to potential customers faster.

🤖 AI Dealership Chatbot

The customer can access an AI chatbot directly from the confirmation email.

The chatbot uses a dealership-specific knowledge base to answer customer questions about the dealership and its available information.

Example questions:

What cars are available?

What is the price of this car?

Do you have SUVs?

What are the available features?

How can I contact the dealership?

The chatbot is designed to provide information based on the dealership's available data rather than generic responses.

🧠 AI Knowledge Base

The chatbot is connected to dealership-specific information.

This allows the AI system to provide answers based on the provided knowledge base.

The knowledge base can contain information such as:

Car models
Prices
Specifications
Available features
Dealership information
Services
Contact information
Frequently asked questions

The chatbot uses the dealership's knowledge base to ground its responses.

🛠️ Technologies
Technology	Purpose
n8n	Workflow automation
Google Sheets	Lead storage
Gmail	Automated email notifications
AI Agent / LLM	Customer interaction
Knowledge Base / RAG	Dealership-specific information
JavaScript	Data processing and transformation
🔧 Main Workflow Components
1. Form Trigger

Receives customer information from the lead form.

2. Data Processing

Cleans and prepares the submitted information.

3. Google Sheets

Stores the new lead automatically.

4. Customer Email

Sends a confirmation message to the customer.

5. Employee Email

Notifies the dealership employee about the new lead.

6. AI Chatbot

Provides customers with an AI-powered way to ask questions about the dealership.