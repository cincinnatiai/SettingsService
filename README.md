# SettingsService

This service manages user-specific configurations and integrates with the Personalized Menu system.

## Architecture

<img width="631" height="340" alt="SettingsService drawio" src="https://github.com/user-attachments/assets/1b33ee62-f249-4a65-868e-5a616aacdad5" />

The system follows a standard three-tier architecture:

1. **Edge:** Cloudflare handles and routes the request.
2. **App Layer:** Spring Boot handles business logic.
3. **Data Layer:** A local database manages persistency.

## Key Features

- **Real-time Offers:** Integrates with StartUpManager service to fetch customized settings.


