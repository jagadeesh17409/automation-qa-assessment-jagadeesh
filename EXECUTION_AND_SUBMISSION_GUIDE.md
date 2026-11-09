# Execute and submit — beginner guide

## Task 1
1. Open https://demo.realworld.io in Chrome.
2. Test sign-up, login, create article, edit, delete, logout.
3. Follow `Task1_QA_Report/TEST_EXECUTION_LOG.md`.
4. Record actual results; use Win+Shift+S for screenshots.
5. Keep only reproduced defects in the final PDF. If a test passes, investigate another edge case.
6. Save screenshots in `Screenshots/`.

## Run n8n on Windows
1. Install Node.js LTS from https://nodejs.org/ if needed.
2. Open Command Prompt and run `npx n8n`.
3. Open http://localhost:5678.
4. Import `Task2_n8n_Workflow/Task2_Workflow_Jagadeesh.json`.
5. Configure Telegram credentials and chat ID in the UI; never add tokens to GitHub.
6. Start webhook test listener and POST `{}` to the test URL shown by n8n. Example:
`curl -X POST http://localhost:5678/webhook-test/github-morning-brief -H "Content-Type: application/json" -d "{}"`
7. Inspect outputs and capture canvas + successful execution screenshots.
8. Import bonus workflow, configure it, test manually, then activate if working.

## Submit
1. Create a PUBLIC GitHub repository named `automation-qa-assessment-jagadeesh`.
2. Upload this folder's contents. Do not upload API tokens, credentials, or .env files.
3. Record a Loom video explaining the QA test cases/findings, API choices, workflow nodes, IF threshold, error handling, and bonus monitor.
4. Make the video viewable by reviewers.
5. Submit the public GitHub URL, brief documentation (under one page), and Loom video URL as required by the assessment.

## Fresher explanation
"I am a fresher, so I broke the assessment into test cases and small workflow steps. I used public APIs, documented assumptions, and focused on understandable error handling. I can explain each test and workflow node. I have clearly separated verified results from scenarios that still need reproduction."

n8n node options can differ by version. Inspect nodes after import and test before activation.
