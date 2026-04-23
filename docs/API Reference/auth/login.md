### <span class="badge badge-post">POST</span> <span class="endpoint">/auth/login</span>

    Get a token with login and password
---

#### Example Request

##### Headers

| Header | Required | Value |
|------|------|------|
| Content-Type | Yes | application/json |

##### Body

```json
{
  "identifier": "username",
  "password": "password"
}
```

---

#### Example Response

```json
{
  "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9...",
  "refresh_token": "0640a4f91e5fb6caa...",
  "user": {
    "id": 0,
    "email": "example@example.com",
    "username": "Example",
    "role": "player",
    "status": 1, // unknown
    "balance": 0,
    "tier": "free",
    "date_of_birth": "2000-01-01",
    "created_at": 1776959564
  }
}
```
