# UMAR Live Bridge

Deployment-ready starter for the persistent UMAR bridge.

## Required environment variables
- NOTION_TOKEN
- CLICKUP_TOKEN
- DATABASE_URL
- NOTION_WEBHOOK_SECRET
- CLICKUP_WEBHOOK_SECRET

## Endpoints
- GET /health
- GET /status
- POST /webhooks/notion
- POST /webhooks/clickup

## Production sequence
1. Deploy this service to Railway.
2. Add secrets as environment variables.
3. Verify /health.
4. Configure Notion and ClickUp webhooks to the public HTTPS endpoints.
5. Implement authenticated adapter calls and mapping storage.
6. Run live execute -> observe -> verify tests.
