---
title: User
---

### <span class="badge badge-get">GET</span> <span class="endpoint">/users/:id/profile</span>

    Get user profile

#### Parameters
| Parameter | Description | Type |
|-----|-----|-----|
| id | Luduvo User ID | Path |

---

#### Authentication

| Type | Required |
|-----|-----|
| None | N/A |

---

#### Example Response

```json
{
  "user_id": 0,
  "username": "Example",
  "member_since": 1775090555,
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
  "last_active": 1775090555,
  "allow_joins": true,
  "is_owner": false // indicates whether you are owner of this resource
}
```