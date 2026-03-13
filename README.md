# CeProMinDB — Mining Events Database 2026

**Last updated: March 12, 2026**

A curated JSON database of global mining conferences, exhibitions, symposiums, and investment forums for 2026, with an interactive HTML dashboard for visualization.

## Contents

| File | Description |
|---|---|
| `mining_events.json` | Source database — 54 events with full metadata |
| `index.html` | Self-contained interactive dashboard (no build step) |

## Dashboard Features

- **Stat cards** — total events, upcoming/past counts, regions, countries, largest event by attendance
- **Charts** — regional distribution (doughnut), events by month (bar), top commodities (horizontal bar)
- **Timeline** — all 12 months with color-coded event strips by type
- **Filterable table** — search by name/city/organizer; filter by region, type, status, commodity; sortable columns
- **Event modal** — click any event for full details (venue, attendance, focus areas, website link)

Open `index.html` directly in a browser — no server or dependencies required (Chart.js loaded from CDN).

## Database Schema

Each event in `mining_events.json` follows this structure:

```json
{
  "id": 1,
  "name": "Event Full Name",
  "type": "Conference / Exhibition / Forum / ...",
  "start_date": "2026-MM-DD",
  "end_date": "2026-MM-DD",
  "city": "City",
  "country": "Country",
  "venue": "Venue Name",
  "organizer": "Organizer Name",
  "website": "https://...",
  "focus": ["topic 1", "topic 2"],
  "commodities": ["gold", "copper", "lithium"],
  "region": "Latin America",
  "status": "upcoming",
  "attendance": 5000,
  "exhibitors": 200,
  "notes": "Optional notes"
}
```

### Regions

`North America` · `Latin America` · `Europe` · `Africa` · `Asia` · `Asia-Pacific` · `Global`

### Status values

- `upcoming` — event has not yet occurred
- `past` — event has already taken place

## Coverage

**54 events** across 6 regions and 25+ countries — January through December 2026.

Highlights:
- **Largest event:** bauma CHINA 2026 — 281,000 attendees (Shanghai, Nov)
- **Largest exploration convention:** PDAC 2026 — 32,155 attendees, 1,300 exhibitors (Toronto, Mar)
- **Argentina focus:** Expo San Juan Minera, Argentina Rocks, Argentina Week NYC, Direct Lithium Extraction
- **Peru focus:** SIMPOSIO XVI (SNMPE), EXPOCOBRE, World Mining Congress

## Sources

Event data sourced from official event websites, industry publications, and organizer announcements. Key sources include:
- [Panorama Minero](https://www.panorama-minero.com)
- [AusIMM](https://www.ausimm.com)
- [SAIMM](https://www.saimm.co.za)
- [Mining.com](https://www.mining.com)
- Individual event websites listed in each record

---
