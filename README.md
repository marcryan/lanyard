# Lanyard

Mobile-first web app for quickly looking up players by jersey number from the 2026 Varsity Roster.

Repo: [marcryan/lanyard](https://github.com/marcryan/lanyard) · Live site: [marcryan.github.io/lanyard](https://marcryan.github.io/lanyard)

## Features
- **Big, readable fonts** optimized for mobile devices and quick glances
- **Live search** — type the number and results appear instantly
- **Search by Name** — type a player's name to see their number
- **Multiple Rosters** — supports multiple rosters enabling one app for multiple sports/teams
- **Color-coded class years**: 
  - Senior → emerald green
  - Junior → sky blue  
  - Sophomore → amber
  - Freshman → pink
- Fully self-contained single `index.html` file (no build step)
- Works great on phones, tablets, or desktop

## How to Use
1. Open `index.html` directly in any modern browser (double-click or File → Open).
2. On mobile: transfer the file via AirDrop, email, or USB, then open in Safari/Chrome.
3. For best experience on phone, you can host it:
   - Python: `python3 -m http.server 8080` then visit `http://your-ip:8080`
   - Or upload the single HTML file to any static host (Netlify, Vercel, GitHub Pages, etc.)

## Data
- Roster Manifest registers the avilable rosters 
- Individual rosters stored separately in json
- Live editing: add players dynamically and request roster changes
- Dynamic Updating: monitors source and prompts the user with updated rosters

## Files
- `index.html` — the web app (self-contained)
- `rosters/` — roster data: `roster-app-*.json` (app-format rosters the lookup fetches), `roster_*.json` (raw CIAC exports), `rosters.json` (roster-list manifest)
- `images/` — favicons and source/master assets

Designed for speed and readability on the field or in the stands.
