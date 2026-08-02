# Batch Processing RSS Feed Workflow

## Overview

This n8n workflow demonstrates how to process multiple RSS feed URLs in batches. It uses the **Loop Over Items** node to iterate through each RSS feed URL and the **RSS Feed Read** node to retrieve articles from every feed.

This approach is useful because the RSS Feed Read node processes one feed URL at a time.

## Workflow

1. Manual Trigger starts the workflow.
2. FeedURLs provides a list of RSS feed URLs.
3. Loop Over Items processes each feed URL individually.
4. RSS Feed Read retrieves articles from the current RSS feed.
5. The loop continues until all feed URLs have been processed.

## Nodes Used

- Manual Trigger
- Code
- Loop Over Items
- RSS Feed Read

## Output

The workflow returns the latest articles from all configured RSS feeds.

Each output item contains information such as:

- Article title
- Link
- Publication date
- Description

Example:

```json
{
  "title": "Latest AI News",
  "link": "https://example.com/article",
  "pubDate": "2026-08-02",
  "description": "Article summary..."
}
```

## Files Included

- `Batch-processing-RSS-feeds.json` — n8n workflow
- `batch-processing-RSS-feed.png` — Workflow screenshot

## Skills Demonstrated

- Batch processing
- Loop Over Items
- RSS feed integration
- Processing multiple data sources
- Workflow automation
- Data extraction from XML feeds
