# Merging Customer Data Workflow

## Overview

This n8n workflow demonstrates how to merge customer records with country information from two different data sources. It combines customer data with matching country details and updates the resulting records.

This workflow showcases how to enrich existing datasets by merging related information before performing further processing.

## Workflow

1. Manual Trigger starts the workflow.
2. GetCustomers retrieves customer records.
3. GetCountries fetches country information from an external API.
4. Merge combines customer records with their corresponding country data.
5. UpdateCustomers outputs the enriched customer dataset.

## Nodes Used

- Manual Trigger
- GetCustomers
- HTTP Request
- Merge
- UpdateCustomers

## Output

The workflow produces customer records enriched with country information.

Example:

```json
{
  "id": 1,
  "name": "John Doe",
  "country": "Canada",
  "countryCode": "CA"
}
```

## Files Included

- `Merging-customer-data.json` — n8n workflow
- `Merging-data.png` — Workflow screenshot

## Skills Demonstrated

- Data merging
- Combining multiple data sources
- HTTP Request integration
- Data enrichment
- Updating structured datasets
- Workflow automation
