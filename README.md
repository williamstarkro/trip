# William Goes South

A journey chart for the Dientes de Navarino trip, Thanksgiving week 2026. Served at https://williamstarkro.github.io/trip/ from the `trip` repo.

Everything is one static page, `index.html`, plus `dispatches.json`.

## Posting a dispatch from your phone

1. Open `dispatches.json` on GitHub (the pencil icon works in the mobile site or the GitHub app).
2. Add an entry at the top of the list:

```json
{ "date": "2026-11-21", "where": "Puerto Williams", "lat": -54.93, "text": "Signed in with the Carabineros. Bought 2 kg of cookies." }
```

3. Commit to `main`. The page refreshes within a minute or two. Newest date shows first. `lat` is optional.

## Previewing a date

Append `?day=2026-11-24` to the URL to see what the chart says on any date. Friends can use it to peek ahead.

## Changing the plan

The itinerary lives in one array, `LEGS`, near the top of the script in `index.html`. Each entry has a date, a title, a status line, and whether there is phone signal that day. The worry meter thresholds are in the `worry()` function just below it.
