# 📊 Generating Reports Workflow

## Overview
This workflow generates business reports from customer and order data. It combines information from multiple sources, calculates order totals, sorts the data, creates region-based summaries, converts reports into CSV files, uploads the full report, and sends a summary to Discord.

## Workflow Steps

1. **Manual Trigger**
   - Starts the workflow manually.

2. **GetOrderData**
   - Retrieves order information from an external API.

3. **GetCustomers**
   - Retrieves customer information.

4. **Merge**
   - Combines customer and order data into a single dataset.

5. **CalculateTotal**
   - Calculates the total value for each order.

6. **SortByTotal**
   - Sorts all orders based on their total value.

7. **EuropeOnly**
   - Filters orders belonging to European customers.

8. **ConvertToCSV**
   - Converts the European orders into a CSV report.

9. **UploadReport**
   - Uploads the generated CSV report to a remote server.

10. **SummarizeByRegion**
    - Groups and summarizes orders by region.

11. **SortSummary**
    - Sorts the regional summary for easier reading.

12. **Convert to CSV**
    - Converts the regional summary into CSV format.

13. **BuildDiscordMessage**
    - Creates a formatted summary message containing key report statistics.

14. **SendToDiscord**
    - Sends the report summary to a Discord channel.

## What This Workflow Demonstrates

- Fetching data from multiple APIs
- Merging datasets
- Data transformation
- Calculating values
- Sorting records
- Filtering data
- Creating summaries
- Generating CSV reports
- Uploading generated reports
- Sending automated notifications to Discord

## Files Included

- `Generating-reports.json` – n8n workflow export
- `Generating-reports.png` – Workflow screenshot
- `README.md` – Workflow documentation
