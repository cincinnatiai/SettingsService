# SettingsService

This service manages user-specific configurations and integrates with the Personalized Menu system.

## Architecture

<img width="631" height="360" alt="SettingsService drawio" src="https://github.com/user-attachments/assets/9918480e-dd5c-4b02-933f-158f305d4bc3" />

The system follows a standard three-tier architecture:

1. **Edge:** Cloudflare handles and routes the request.
2. **App Layer:** Spring Boot handles business logic.
3. **Data Layer:** A local database manages persistency.

## Key Features

- **Real-time Offers:** Integrates with StartUpManager service to fetch customized settings.


