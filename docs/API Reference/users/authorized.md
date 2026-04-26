---
title: Authorized User
---

### <span class="badge badge-get">GET</span> <span class="endpoint">/me/profile</span>

Get authorized user profile

#### Authentication

| Type | Required |
|-----|-----|
| Bearer | Yes |

#### Example Response

```json
{
  "user_id": 0,
  "username": "Example",
  "member_since": 1776959901,
  "networth": 0,
  "display_name": null,
  "status": null,
  "bio": null,
  "avatar": {
    "head_color": "#C8C8C8",
    "torso_color": "#23590A",
    "left_arm_color": "#C8C8C8",
    "right_arm_color": "#C8C8C8",
    "left_leg_color": "#8E5226",
    "right_leg_color": "#8E5226"
  },
  "accent_color": null,
  "banner_url": "",
  "equipped_items": [],
  "badges": [],
  "friend_count": 0,
  "place_count": 0,
  "item_count": 0,
  "last_active": 1776959901,
  "allow_joins": true,
  "is_owner": false
}
```

---


### <span class="badge badge-put">PUT</span> <span class="endpoint">/me/profile</span>

Update user's profile

#### Authentication

| Type | Required |
|-----|-----|
| Bearer | Yes |

#### Example Request

##### Headers

| Header | Required | Value |
|------|------|------|
| Content-Type | Yes | application/json |

##### Body

```json
{
  "bio": "Example"
}
```

!!! info 
    Currently known available parameters to edit are `display_name`, `bio`, `status`, `allow_joins`, and `accent_color`.
    
    All parameters in the `avatar` table are available to edit, however they must be outside of the `avatar` table.

!!! note
    If a parameter is not provided in the request body, it will be set to `null` or a predefined default value.

#### Example Response

```json
{
  "user_id": 0,
  "username": "Example",
  "member_since": 1776959901,
  "networth": 0,
  "display_name": null,
  "status": null,
  "bio": "Example",
  "avatar": {
    "head_color": "#C8C8C8",
    "torso_color": "#23590A",
    "left_arm_color": "#C8C8C8",
    "right_arm_color": "#C8C8C8",
    "left_leg_color": "#8E5226",
    "right_leg_color": "#8E5226"
  },
  "accent_color": null,
  "banner_url": "",
  "equipped_items": [],
  "badges": [],
  "friend_count": 0,
  "place_count": 0,
  "item_count": 0,
  "last_active": 1776959901,
  "allow_joins": true,
  "is_owner": false
}
```

---

### <span class="badge badge-get">GET</span> <span class="endpoint">/me/friends</span>

Get authorized user friends

#### Authentication

| Type | Required |
|-----|-----|
| Bearer | Yes |

#### Example Response

```json
{
  "items": [],
  "total": 0,
  "limit": 50,
  "offset": 0
}
```

---

### <span class="badge badge-get">GET</span> <span class="endpoint">/me/inventory</span>

Get authorized user inventory

!!! note
    This appears to be identical to <span class="badge badge-get">GET</span> <span class="endpoint">/me/friends</span>.

#### Authentication

| Type | Required |
|-----|-----|
| Bearer | Yes |

#### Example Response

```json
{
	"items": [],
	"total": 0,
	"limit": 50,
	"offset": 0
}
```

---

### <span class="badge badge-get">GET</span> <span class="endpoint">/me/items</span>

Get authorized user items

!!! note
    This appears to be identical to <span class="badge badge-get">GET</span> <span class="endpoint">/me/inventory</span>.

#### Authentication

| Type | Required |
|-----|-----|
| Bearer | Yes |

#### Example Response

```json
{
	"items": [],
	"total": 0,
	"limit": 50,
	"offset": 0
}
```
