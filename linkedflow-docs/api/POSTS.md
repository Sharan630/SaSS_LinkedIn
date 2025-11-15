# Posts API

## Endpoints

### POST /generation/posts

Generate a new LinkedIn post using AI.

**Request Body:**
```json
{
  "topic": "AI in Marketing",
  "tone": "professional",
  "length": "medium",
  "includeHashtags": true
}
```

**Response:**
```json
{
  "id": 1,
  "content": "Generated post content...",
  "hashtags": ["#AI", "#Marketing"],
  "createdAt": "2024-01-01T00:00:00Z"
}
```

### GET /generation/posts

Get all generated posts for the authenticated user.

### GET /generation/posts/:id

Get a specific post by ID.

### PUT /generation/posts/:id

Update a post.

### DELETE /generation/posts/:id

Delete a post.

