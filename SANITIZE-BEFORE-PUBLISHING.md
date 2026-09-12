# Before Publishing

Do NOT publish the raw n8n export without reviewing it.

1. Open `workflow/ai-research-agent-raw.json` locally.
2. Remove credential references and n8n instance-specific metadata.
3. Save the cleaned copy as `workflow/ai-research-agent-sanitized.json`.
4. Search the file for:
   - `credentials`
   - `apiKey`
   - `token`
   - `password`
   - `webhookId`
   - `instanceId`
5. Confirm there are no real secrets or private identifiers.
6. Only commit the sanitized file.
