# Sanitization Notes

The public copies remove instance-specific and account-specific data while preserving workflow structure and expressions.

Removed or changed where present:

- n8n root `id`, `versionId`, and `meta.instanceId`
- node `webhookId`
- node `credentials` blocks
- pinned execution data (`pinData`)
- Google account email/calendar references
- Google Sheet IDs and cached URLs
- notification email recipient
- Google Tasks list identifier
- linked workflow identifier
- Pinecone index/namespace identifiers
- personal/sample naming in the lead notification example

Node IDs and workflow logic are retained so the exported JSON remains recognizable and easy to compare with the original.
