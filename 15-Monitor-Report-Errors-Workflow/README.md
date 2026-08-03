# 🚨 Monitor Report Errors Workflow

## Overview
This workflow automatically monitors failed n8n workflow executions. Whenever a workflow encounters an error, it captures the error details, formats a notification message, and sends it to a Discord channel. This enables real-time monitoring and faster troubleshooting without manually checking execution logs.

## Workflow Steps

1. **Error Trigger**
   - Automatically starts when another n8n workflow fails.

2. **BuildErrorMessage**
   - Formats the error information into a readable notification.
   - Includes details such as the workflow name, error message, and execution information.

3. **NotifyDiscord**
   - Sends the formatted error notification to a Discord channel for immediate visibility.

## What This Workflow Demonstrates

- Automatic error monitoring
- Global error handling
- Event-driven workflows
- Formatting error messages
- Discord integration
- Real-time notifications
- Workflow observability

## Files Included

- `Monitor-Report-Errors.json` – n8n workflow export
- `Monitor-errors.png` – Workflow screenshot
- `README.md` – Workflow documentation
