# Settings Service

A microservice designed to manage user specific configurations and system settings.

## Architecture

<img width="656" height="340" alt="Settings drawio" src="https://github.com/user-attachments/assets/6dbc87e8-2ef1-4315-b0ed-3ebad1f5c5b3" />

The system is organized into a modular flow:

1.  **Actor/Client:** Initiates requests via the web, android or iOS app.
2.  **StartupManager Facade:** Acts as the entry point for orchestration and initial service routing.
3.  **Edge Layer:** Cloudflare provides security, caching, and request routing.
4.  **Application Layer (VPC):** A Spring Boot service running within a secure VPC to process business logic.
5.  **Data Layer:** A local database ensuring high availability persistence for user settings.

## Key Features

- **Request Facade:** Uses a StartupManager to abstract initialization logic from the client.
- **Secure Environment:** The core service and database are isolated within a Virtual Private Cloud.
- **Data Consistency:** Reliable persistence using PostgreSQL.
