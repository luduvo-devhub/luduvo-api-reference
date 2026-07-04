### <span class="badge badge-post">GET</span> <span class="endpoint">/me/places</span>

    Get your places
---

#### Example Request

#### Authentication

| Type | Required |
|-----|-----|
| Bearer | Yes |


#### Example Response

```json
{
   "limit" : 50,
   "offset" : 0,
   "places" : [
      {
         "access" : "public",
         "active_players" : 0,
         "created_at" : 1783121887,
         "description" : "",
         "id" : 1,
         "max_players" : 10,
         "owner_id" : 1,
         "owner_username" : "",
         "pending_thumbnail_url" : ".png",
         "thumbnail_status" : "pending",
         "thumbnail_url" : "",
         "thumbs_down" : 0,
         "thumbs_up" : 0,
         "title" : "Example",
         "updated_at" : 1783125713,
         "visit_count" : 0
      }
   ],
   "total" : 1
}
```
