# Planner API

## Endpoints

### GET /planner/weekly

Get weekly content plan.

**Query Parameters:**
- `week` - Week number (ISO week format)

**Response:**
```json
{
  "week": "2024-W01",
  "posts": [
    {
      "id": 1,
      "scheduledDate": "2024-01-01T09:00:00Z",
      "topic": "AI Trends",
      "status": "scheduled"
    }
  ]
}
```

### POST /planner/weekly

Generate a weekly content plan using AI.

**Request Body:**
```json
{
  "goals": ["Increase engagement", "Build thought leadership"],
  "topics": ["AI", "Marketing", "Technology"],
  "postsPerWeek": 5
}
```

### POST /planner/schedule

Schedule a post for a specific date/time.

### GET /planner/calendar

Get calendar view of scheduled posts.

