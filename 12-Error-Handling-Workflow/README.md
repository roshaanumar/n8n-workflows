# Error Handling Workflow

## Overview

This n8n workflow demonstrates how to handle successful and failed API requests using separate execution paths. It uses an HTTP Request node that intentionally calls an endpoint returning an error, allowing the workflow to branch into either a success or error handling path.

This pattern is commonly used in production workflows to improve reliability and prevent unexpected workflow failures.

## Workflow

1. Manual Trigger starts the workflow.
2. HTTP Request sends a GET request to an API endpoint.
3. If the request succeeds, the workflow follows the **Success** branch.
4. If the request fails, the workflow follows the **HandleError** branch.
5. Each branch can perform different actions such as logging, notifications, retries, or recovery.

## Nodes Used

- Manual Trigger
- HTTP Request
- Success (Manual)
- HandleError (Manual)

## Output

Depending on the API response:

### Success

The workflow continues through the success path and processes the returned data.

### Error

The workflow captures the error and executes the error-handling path instead of stopping the workflow.

Example error:

```json
{
  "statusCode": 500,
  "message": "Internal Server Error"
}
```

## Files Included

- `Handling-errors.json` — n8n workflow
- `error-handling.png` — Workflow screenshot

## Skills Demonstrated

- API error handling
- HTTP status codes
- Success and failure branching
- Workflow reliability
- Building fault-tolerant automations
