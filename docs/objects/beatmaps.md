# Beatmap related objects.

## BeatmapData
```json
{
    "id": 75, // The beatmap ID.
    "set_id": 1, // The parent beatmapset id
    "diff_name": "Normal",
    "ar": 6.0, // The approach rate of the difficulty
    "bpm": 120.0,
    "hp": 6.0,
    "od": 6.0,
    "max_combo": 314, // Perfect combo
    "length": 144, // In seconds
    "drain": 109, // In seconds,
    "playcount": 142,
    "passcount": 26,
    "rating": 9.6, // out of 10
    "favourites": 0, // How many people have favourited the map
    "rank_requests": 0, // How many people have requested this map to be ranked
    "uploaded": 0, // Unix timestamp for when it was uploaded
    "updated": 0, // Unix timestamp for when it was last updated
}
```

## BeatmapsetData
```json
{
    "id": 1, // Beatmapset ID
    "artist": "Kenji Ninuma",
    "title": "DISCO PRINCE",
    "creator": "peppy",
    "maps" : [
        BeatmapData...
    ]
}
```
