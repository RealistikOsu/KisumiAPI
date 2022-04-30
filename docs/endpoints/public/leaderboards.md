# Leaderboard Related Endpoints

## GET /api/v3/leaderboards
### GET Arguments
- `page` - The page of the search. Defaults to 0
- `c_mode` - The custom mode enum (0 = VN, 1 = RX, 2 = AP). Defaults to 0.
- `mode` - The osu! mode enums (0 = standard...). Defaults to 0.
- `order` - The ordering factor for the leaderboard (score/pp). Defaults to pp.
- `results` - How many results should be in a page. Max 100. Defaults to 50.

### Sample response.
```json
{
    "total_players": 2000, // For help with pagination
    "player_count": 50, // Amount of results in this reponse. Max `results` GET arg.
    "players" [PlayerCardData], // Ordered by `order`
}
