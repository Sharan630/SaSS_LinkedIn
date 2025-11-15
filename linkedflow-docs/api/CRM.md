# CRM API

## Endpoints

### GET /crm/contacts

Get all contacts/leads.

**Query Parameters:**
- `page` - Page number
- `limit` - Items per page
- `search` - Search query

### POST /crm/contacts

Create a new contact.

**Request Body:**
```json
{
  "name": "John Doe",
  "email": "john@example.com",
  "company": "Example Corp",
  "linkedinUrl": "https://linkedin.com/in/johndoe",
  "tags": ["lead", "prospect"]
}
```

### GET /crm/contacts/:id

Get a specific contact.

### PUT /crm/contacts/:id

Update a contact.

### DELETE /crm/contacts/:id

Delete a contact.

### POST /crm/contacts/:id/interactions

Add an interaction/note to a contact.

