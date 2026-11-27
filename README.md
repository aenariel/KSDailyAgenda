# KSDailyAgenda

Daily agenda generator for Kingshot alliances: picks the day's events from the 28-day cycle and builds two ready-to-paste messages
(the alliance "Group info" message and a compact "Normal message" for group chats).

Live page: https://aenariel.github.io/KSDailyAgenda/

## Files

- `index.html` – the whole app (no build step, no server). Your alliances, times and daily notes are stored in your own browser (localStorage).
  Use *Backup and reset → Show everything / Import* to move your data to another browser or device.
- `events.json` – the fixed events shared by every kingdom (Brawl, Strongest Governor, KvK, Castle Battle…).
  When editing it, **increase `version`**: open pages then replace their fixed events with the new list, keeping each user's on/off ticks.

## Notes

- Dates use the game's UTC day. The cycle start (`anchor`) is the Monday of an Alliance Brawl week.
- Kingdom-specific events (Fishing Tournament, Mystic Divination, Desert Trial / Champion's Way…) are edited in the page and stay local.
- Kingdoms are named by number with `#` (`#1130`); older names like `K1130` are renamed when the page opens.
- Sanctuary & Fortress battles are on Fridays at the slot most voted at sign-up: 3, 9, 13, 14 or 17 UTC. Until a battle is picked, Friday shows "time TBD".
