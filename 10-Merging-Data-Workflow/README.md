# Merging Data Workflow

## Overview

This n8n workflow demonstrates how to merge data from two different sources into a single output using the **Merge** node.

The workflow retrieves customer information from one source and character data from another source, then combines both datasets into a unified result.

## Workflow

1. Manual Trigger starts the workflow.
2. GetCustomerData retrieves customer records.
3. Characters generates a second dataset.
4. Merge combines both inputs into a single output.

## Nodes Used

- Manual Trigger
- GetCustomerData
- Code
- Merge

## Output

The workflow produces merged records containing information from both input datasets.

Example:

```json
{
  "customer": {
    "id": 1,
    "name": "John Doe"
  },
  "character": {
    "name": "Mario"
  }
}
```

> The actual output depends on the data provided to the Merge node.

## Files Included

- `merging-data.json` — n8n workflow
- `merging-data.png` — Workflow screenshot

## Skills Demonstrated

- Data merging
- Combining multiple data sources
- Workflow branching
- Data transformation
- n8n Merge node
