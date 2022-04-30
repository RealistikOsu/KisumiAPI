# Player related object

## RoleData
```json
{
    "id": 1,
    "name": "Owner",
    "colour": "#4287f5", // Hex
    "privileges": 7, // Bitwise enum
}
```

## UserStatsData
```json
{
    "total_score": 0,
    "ranked_score": 0,
    "pp": 0.0,
    "play_count": 0,
    "play_time": 0, // In minutes
    "accuracy": 100.0, // Max is 100
    "max_combo": 0,
    "rank": 0 // 0 means unranked
}
```

## PlayerCardData
```json
{
    "id": 1000,
    "name": "RealistikDash",
    "roles": [RoleData],
    "stats": {
        0: [UserStatsData] // Index of the array is the mode enum value (eg standard = 0)
        // Repeat 0..3 (vn, rx, ap)
    },
    "clan": {
        "id": 1,
        "tag": "GANG",
        "name": "Official[GANG]"
    },
    "background_url": "/static/headers/leaderboard2.jpg",
    "supporter": true, // Whether the user is a supporter
    "verified": true, // Whether the user is verified as legit
}
```