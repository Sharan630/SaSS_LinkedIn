# Analytics API

## Endpoints

### GET /analytics/overview

Get analytics overview for the authenticated user.

**Response:**
```json
{
  "totalPosts": 150,
  "totalEngagement": 5000,
  "averageEngagement": 33.3,
  "topPerformingPosts": [...],
  "engagementTrend": [...]
}
```

### GET /analytics/posts/:id

Get analytics for a specific post.

### GET /analytics/trends

Get engagement trends over time.

**Query Parameters:**
- `startDate` - Start date (ISO format)
- `endDate` - End date (ISO format)
- `metric` - Metric to analyze (engagement, views, likes)

