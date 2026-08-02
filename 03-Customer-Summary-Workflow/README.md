# Customer Summary Workflow

## Overview

This n8n workflow retrieves customer records, counts the total number of customers, and generates a summary of the retrieved data.

## Workflow Steps

1. **Manual Trigger** – Starts the workflow manually.
2. **GetCustomers** – Fetches all customer records from the data source.
3. **CountCustomers** – Counts the total number of customers using a Code node.
4. **SetSummary** – Creates a structured summary of the results.

## Features

- Retrieves customer data
- Counts total customers
- Generates a concise summary
- Demonstrates data transformation using Code and Set nodes

## Technologies Used

- n8n
- Code Node (JavaScript)
- Set Node
- Data Source Integration
- JSON

## Files

| File | Description |
|------|-------------|
| `customer-summary-workflow.json` | Importable n8n workflow |
| `customer-summary-workflow.png` | Screenshot of the workflow |

## Screenshot

![Workflow](customer-summary-workflow.png)
