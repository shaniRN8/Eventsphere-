# Eventsphere

This repository contains the backend implementation for Eventsphere, an event management system built with pure Java Servlets and deployed on GlassFish Server

🚀 Features
User authentication and event management APIs

Ticket purchase and Stripe payment integration

File and media storage with Azure Blob Storage

SQL database hosted in Azure SQL Database

Resource scripts available to set up schema and tables

🛠️ Tech Stack
Backend: Java Servlets

Server: GlassFish

Database: Azure SQL Database

Storage: Azure Blob Storage

Payment: Stripe

⚙️ Setup & Installation
1. Clone the Repository
   git clone https://github.com/SandunPushpika/EventsphereBackend.git
   cd eventsphere-backend
2. Database Setup
The SQL scripts for schema and tables are available in the resources/ folder.

Run these scripts on your Azure SQL Database.

3. Environment Variables
Create a .env file in the root directory with the following values:

DB_URL=jdbc:sqlserver://<your-db-server>.database.windows.net:1433;database=<dbname>
DB_USER=<your-db-username>
DB_PASSWORD=<your-db-password>

AZURE_BLOB_CONNECTION_STRING=<your-azure-blob-connection-string>
AZURE_BLOB_CONTAINER=<your-container-name>

STRIPE_SECRET_KEY=<your-stripe-secret-key>
STRIPE_PUBLIC_KEY=<your-stripe-public-key>
Note: .env is included here only because this is not a commercial project. In production, environment variables should be securely managed and excluded from source control.

4. Deploy to GlassFish
Build the project and generate a WAR file.

Deploy the WAR to your GlassFish server.

Start the server and access the backend at: http://localhost:8080/eventsphere

💳 Payment Integration
Payments are handled via Stripe.

Stripe keys are configured in the .env file.

Test keys can be used during development.

☁️ Storage
Event-related assets (images, documents, etc.) are stored in Azure Blob Storage.

Make sure the container specified in .env exists before running the project.

📜 License
This project is for educational purposes and not intended for commercial use.
