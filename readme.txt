✨ Features
📝 Lead Generation

Customers submit their information through a dealership lead form.

Collected information includes:

Name
Phone number
Email
Request type
Preferred car type
Budget
Notes
Preferred contact time
⚙️ Automated Lead Processing

The submitted information is processed and organized automatically before being stored.

This removes repetitive manual data-entry work and keeps incoming leads structured.

📊 Google Sheets Integration

Every submitted lead is automatically added to Google Sheets.

Example:

Name	Phone	Email	Car Type	Budget	Request
Ahmed	010xxxxxxx	ahmed@email.com	Sedan	1,200,000 EGP	Buy

The sales team can use the sheet to track and manage incoming customer requests.

📧 Customer Confirmation

After submitting the form, the customer automatically receives a confirmation email.

The email:

Confirms that the request was received
Provides basic information
Contains a link to the AI dealership chatbot

Example:

Thank you for contacting us. Your request has been received successfully.

You can also chat with our AI assistant to learn more about available cars, prices, specifications, and dealership information.

👨‍💼 Employee Notification

A new-lead notification is automatically sent to the dealership employee.

The notification contains the customer's submitted information, allowing the sales team to follow up quickly.

🤖 AI Dealership Chatbot

Customers can access the AI chatbot directly from the confirmation email.

The chatbot is connected to a dealership-specific knowledge base and can answer questions such as:

What cars are available?

How much is the BMW?

Do you have SUVs?

What are the car specifications?

What features does this model have?

How can I contact the dealership?

Instead of relying only on general LLM knowledge, the chatbot uses dealership-specific information to provide more relevant responses.

🧠 Knowledge Base & RAG

The chatbot can be connected to a dealership knowledge base containing:

🚘 Car models
💰 Prices
⚙️ Specifications
✨ Features
🏢 Dealership information
📞 Contact information
❓ Frequently asked questions

The architecture can use Retrieval-Augmented Generation (RAG) to retrieve relevant dealership information before generating an answer.

Customer Question
       │
       ▼
   AI Chatbot
       │
       ▼
Retrieve Relevant Data
       │
       ▼
Dealership Knowledge Base
       │
       ▼
    LLM Response
       │
       ▼
    Customer
🛠️ Tech Stack
Technology	Purpose
n8n	Workflow automation
Google Sheets	Lead storage
Gmail	Automated email communication
AI Agent	AI-powered customer interaction
LLM	Natural language understanding & generation
RAG / Knowledge Base	Dealership-specific information
JavaScript	Data processing & transformation
🔄 Workflow Components
1. Lead Form

Receives customer information.

2. Data Processing

Validates and prepares the submitted lead data.

3. Google Sheets

Stores the processed lead.

4. Customer Email

Sends an automatic confirmation and chatbot link.

5. Employee Notification

Alerts the sales team about the new lead.

6. AI Chatbot

Answers customer questions using dealership information.

📂 Project Structure
ai-lead-chatbot/
│
├── README.md
├── workflow.json
│
└── screenshots/
    ├── workflow.png
    └── chatbot.png
📸 Screenshots
n8n Workflow

AI Dealership Chatbot

Google Sheets

🚀 Getting Started
1. Import the Workflow

Import the workflow.json file into your n8n instance.

2. Configure Credentials

Connect the required services:

Google Sheets
Gmail
AI provider
Any other services used by the workflow
3. Configure the Lead Form

Make sure the form fields match the workflow input fields.

4. Configure the Knowledge Base

Add the dealership's data that should be available to the AI chatbot.

5. Test the Workflow

Submit a test lead and verify:

Lead processing
Google Sheets storage
Customer confirmation email
Employee notification
Chatbot access
AI responses
🔐 Security

Sensitive information should never be committed to the repository.

Do not upload:

API keys
Passwords
Access tokens
OAuth credentials
Private credentials
Real customer information

Before uploading workflow.json, make sure credentials and sensitive data have been removed.

🎯 Project Goals

This project demonstrates how AI and workflow automation can be combined to improve the customer acquisition process of a car dealership.

The system helps the dealership:
⚡ Capture leads automatically
📊 Keep lead information organized
📧 Communicate with customers automatically
🔔 Notify sales employees instantly
🤖 Provide AI-powered customer support
⏱️ Reduce repetitive manual tasks
📈 Create a foundation for scalable sales automation
🔮 Future Improvements

Potential extensions include:

 AI lead scoring
 Lead qualification
 Automated follow-up
 CRM integration
 Appointment booking
 Vehicle inventory integration
 Sales analytics dashboard
 Conversation history
 Human-agent handoff
 WhatsApp / Instagram / Facebook integration
👨‍💻 Author

Nour Zaki
