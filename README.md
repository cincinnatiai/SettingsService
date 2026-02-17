# SettingsService

This service manages user-specific configurations and integrates with the Personalized Menu system.

## Architecture

<img width="631" height="359" alt="ServiceSettings drawio" src="https://github.com/user-attachments/assets/4204529b-a4aa-4e20-9cc7-16af8ee6998e" />

The system follows a standard three-tier architecture:

1. **Edge:** Cloudflare handles and routes the request.
2. **App Layer:** Spring Boot handles business logic.
3. **Data Layer:** A local database manages persistency.

## Key Features

- **Real-time Offers:** Integrates with StartUpManager service to fetch customized settings.


