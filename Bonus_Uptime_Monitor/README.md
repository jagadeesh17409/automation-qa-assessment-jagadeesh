# Bonus — Uptime monitor

Imports a Schedule Trigger (every 5 minutes), checks `https://demo.realworld.io`, tests for HTTP 200, and sends a Telegram alert on non-200/error.

Setup:
1. Import `Bonus_UptimeMonitor_Jagadeesh.json`.
2. Configure Telegram credentials and chat ID.
3. Run manually; verify 200 path.
4. Temporarily use an invalid URL to test alert path, then restore the real URL.
5. Activate after testing and capture a canvas screenshot.
