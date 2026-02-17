# Settings Service

A high-performance microservice designed to manage user-specific configurations and system settings.

## Architecture

<img width="631" height="340" alt="SettingsServices drawio" src="https://github.com/user-attachments/assets/9cc34bab-0b3f-4882-96d6-3afaec9629fa" />

The system is organized into a modular flow:

1.  **Actor/Client:** Initiates requests via the web, android or iOS app.
2.  **StartupManager Facade:** Acts as the entry point for orchestration and initial service routing.
3.  **Edge Layer:** Cloudflare provides security, caching, and request routing.
4.  **Application Layer (VPC):** A Spring Boot service running within a secure VPC to process business logic.
5.  **Data Layer:** A local database ensuring high-availability persistence for user settings.

## Key Features

* **Request Facade:** Uses a StartupManager to abstract initialization logic from the client.
* **Secure Environment:** The core service and database are isolated within a Virtual Private Cloud.
* **Data Consistency:** Reliable persistence using PostgreSQL.
