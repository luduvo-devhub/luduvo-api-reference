### &lt;span class="badge badge-get"&gt;GET&lt;/span&gt; &lt;span class="endpoint"&gt;/me/recently-played&lt;/span&gt;
```
Get the authenticated user's recently played places
```

---

#### Authentication

| Type                    | Required |
| ----------------------- | -------- |
| Cookie (`sessionToken`) | Yes      |

---

#### Example Request

##### Query Parameters

| Parameter | Required | Value |
| --------- | -------- | ----- |
| limit     | No       | 50    |
| offset    | No       | 0     |

---

#### Example Response
```
{
  "places": [
    {
      "place_id": 2967,
      "title": "Just a baseplate",
      "owner_id": 13422,
      "owner_username": "jigsaw",
      "access": "public",
      "thumbnail_url": "https://assets.luduvo.com/place-thumbnails/fe7a26f0-3c0f-4e4b-8d8f-a8d75f0bda3c.png",
      "square_thumbnail_url": "https://assets.luduvo.com/place-thumbnails/e82dd5d9-c75c-4916-a0d4-ecee293644d4.png",
      "active_players": 0,
      "last_played_at": 1794778273,
      "playtime_seconds": 0,
      "sessions": 1,
      "thumbs_up": 0,
      "thumbs_down": 0
    }
  ],
  "limit": 50,
  "offset": 0
}
```
