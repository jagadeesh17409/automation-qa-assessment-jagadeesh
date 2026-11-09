# Task 2 — GitHub morning brief workflow

What it does:
1. Webhook trigger.
2. HTTP Request calls GitHub Search API for JavaScript repositories.
3. Code node sorts by stars and keeps top five.
4. HTTP Request enriches the highest-ranked repository.
5. IF checks whether stars >= 1,000.
6. Telegram sends a high-priority or normal digest.

Setup:
1. Run `npx n8n`, open http://localhost:5678.
2. Workflows → Import from File → select `Task2_Workflow_Jagadeesh.json`.
3. Create Telegram bot with BotFather, add it to a chat/group, obtain chat ID.
4. Create Telegram credentials in n8n. Select the credential in both Telegram nodes and replace the chat ID placeholder. Never commit secrets.
5. Start the Webhook node's test listener and POST `{}` to its test URL.
6. Inspect every node output. Capture a workflow canvas screenshot and a successful execution screenshot.

API choices: GitHub Search API provides public repository metadata and stars. The repository endpoint enriches the top repository with description, language, URL, and star count. Telegram is the notification channel.

Error handling: HTTP nodes use continue-on-fail where supported; inspect errors in execution output and ensure the fallback message is used. Node settings may vary by n8n version; verify after import. Workflow is inactive by default.
