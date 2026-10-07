# n8n Automation Portfolio

GitHub-ready n8n workflow exports with account-specific credentials, private identifiers, instance metadata, and pinned execution data removed.

## Workflows

| Workflow | Purpose | Main integrations |
|---|---|---|
| `google-calendar-agent.json` | AI assistant for calendar actions and event lookup | n8n, OpenAI, Google Calendar |
| `personal-assistant-using-telegram.json` | Telegram personal assistant with text and voice input | Telegram, OpenAI, Google Tasks, Google Calendar |
| `rag-knowledge-base-agent.json` | RAG assistant that retrieves information from a vector store | n8n chat, OpenAI, Pinecone |
| `agentic-task-assistant.json` | Task-focused AI assistant | n8n chat, OpenAI, Google Tasks |
| `lead-enrichment-and-notification.json` | Lead enrichment and notification workflow | Google Sheets, public enrichment APIs, OpenAI, Gmail |
| `telegram-ai-reply-assistant.json` | AI-powered Telegram reply assistant with memory | Telegram, OpenAI, DeepSeek |
| `shipment-data-cleaner.json` | Shipment validation, duplicate detection, routing and summary | HTTP Request, JavaScript, Switch, Merge |

## Important

These exports are templates. They intentionally do not include working credentials or private account/resource identifiers.

Before activating a workflow, reconnect the required credentials and replace placeholders such as:

- `YOUR_GOOGLE_CALENDAR_ID`
- `YOUR_GOOGLE_SHEET_ID`
- `YOUR_GOOGLE_SHEET_NAME`
- `YOUR_NOTIFICATION_EMAIL`
- `YOUR_GOOGLE_TASK_LIST_ID`
- `YOUR_CALENDAR_WORKFLOW_ID`
- `YOUR_PINECONE_INDEX`
- `YOUR_PINECONE_NAMESPACE`

## Security

Never commit:

- `.env` files
- API keys or tokens
- OAuth secrets
- database passwords
- Telegram bot tokens
- private customer/lead data
- production webhook URLs or secrets
- n8n encryption keys

## Importing

1. Open n8n.
2. Import the JSON file from `workflows/`.
3. Reconnect the credentials for the imported nodes.
4. Replace the placeholders with your own resources.
5. Test each workflow before activation.
