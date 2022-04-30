# Homepage endpoints.

## GET /api/v3/home/status
### GET Args
### Sample Response
```json
{
    "online": 21, // Currently online users
    "registered": 7227, // Total registered users
    "history": {
        "interval": 5, // The time in minutes between each data point.
        "data": [21, 20, 17, 18...]
    },
    "top_plays": [TopPlayData]
}
```