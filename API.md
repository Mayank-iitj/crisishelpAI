# API Documentation

This document outlines the API endpoints and data structures used by the Crisis Helpline platform.

## Base URL

```
https://api.crisishelpline.com/v1
```

## Authentication

Most endpoints require authentication using API keys or JWT tokens.

```javascript
// Example authentication header
headers: {
  'Authorization': 'Bearer your_jwt_token_here',
  'Content-Type': 'application/json'
}
```

## Endpoints

### Chat Support

#### Start Chat Session
```
POST /chat/start
```

**Request Body:**
```json
{
  "userId": "string",
  "urgencyLevel": "low|medium|high|crisis"
}
```

**Response:**
```json
{
  "sessionId": "string",
  "status": "active",
  "estimatedWaitTime": "number (minutes)"
}
```

#### Send Message
```
POST /chat/message
```

**Request Body:**
```json
{
  "sessionId": "string",
  "message": "string",
  "timestamp": "ISO 8601 string"
}
```

### Emergency Services

#### Get Emergency Contacts
```
GET /emergency/contacts?location={country_code}
```

**Response:**
```json
{
  "contacts": [
    {
      "name": "National Suicide Prevention Lifeline",
      "number": "988",
      "description": "24/7 crisis support",
      "languages": ["en", "es"]
    }
  ]
}
```

### Mood Tracking

#### Submit Mood Entry
```
POST /mood/entry
```

**Request Body:**
```json
{
  "userId": "string",
  "mood": "number (1-10)",
  "notes": "string",
  "timestamp": "ISO 8601 string"
}
```

### Resources

#### Get Resources
```
GET /resources?category={category}&language={lang}
```

**Response:**
```json
{
  "resources": [
    {
      "id": "string",
      "title": "string",
      "description": "string",
      "url": "string",
      "category": "string",
      "language": "string"
    }
  ]
}
```

## Error Handling

All API endpoints return standard HTTP status codes:

- `200` - Success
- `400` - Bad Request
- `401` - Unauthorized
- `403` - Forbidden
- `404` - Not Found
- `500` - Internal Server Error

**Error Response Format:**
```json
{
  "error": {
    "code": "string",
    "message": "string",
    "details": "object (optional)"
  }
}
```

## Rate Limiting

API requests are limited to:
- 100 requests per minute for authenticated users
- 20 requests per minute for unauthenticated users

## WebSocket Connections

Real-time chat functionality uses WebSocket connections:

```javascript
const socket = new WebSocket('wss://api.crisishelpline.com/chat');

socket.onmessage = function(event) {
  const data = JSON.parse(event.data);
  // Handle incoming messages
};
```

## Data Privacy

All API communications are encrypted using TLS 1.3. Personal data is handled according to our privacy policy and applicable data protection regulations.

