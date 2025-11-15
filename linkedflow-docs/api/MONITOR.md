# Monitor API

## Endpoints

### GET /monitor/mentions

Get all mentions of the user's brand/keywords.

**Query Parameters:**
- `keyword` - Keyword to monitor
- `platform` - Social media platform
- `dateRange` - Date range filter

### GET /monitor/competitors

Get competitor analysis data.

### GET /monitor/trends

Get trending topics and hashtags.

### POST /monitor/alerts

Create a monitoring alert.

**Request Body:**
```json
{
  "keyword": "LinkedFlow AI",
  "platform": "linkedin",
  "alertType": "mention",
  "frequency": "daily"
}
```

