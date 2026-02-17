# SettingsService

This service manages user-specific configurations and integrates with the Personalized Menu system.

## Architecture

<img width="740" height="255" alt="diagram-export-2-17-2026-1_10_42-PM" src="https://github.com/user-attachments/assets/cb26f8e9-1cfa-4bc7-a23a-7474a411228d" />

The system follows a standard three-tier architecture:

1. **Edge:** Cloudflare handles and routes the request.
2. **App Layer:** Spring Boot handles business logic.
3. **Data Layer:** A local database manages persistency.

## Key Features

- **Real-time Offers:** Integrates with StartUpManager service to fetch customized settings.


