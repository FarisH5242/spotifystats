# TrackSpotify

Independent music analytics and playlist intelligence web application.

**Live demo:** https://farish5242.github.io/spotifystats/

## Features
- Spotify OAuth 2.0 PKCE and playlist import; CSV import/export.
- Artist, genre, decade and available audio-feature analytics; artwork and track links.
- Wrapped PNG cards, CSV battles, artist profiles, discovery search links and session collection.
- Artist relationship graph, heuristic Music DNA, manual local snapshots, smart CSV builder and HTML reports.
- Responsive dashboard and founder About tab.

## Run locally
Serve the repository with `python3 -m http.server 8000` and open http://localhost:8000 for CSV and demo features. Spotify login uses the registered production redirect URI.

## Spotify setup
Create a Spotify developer app, register https://farish5242.github.io/spotifystats/ as the exact redirect URI, and enter its Client ID in the dashboard. Never commit a client secret or access token. Access depends on Spotify app permissions. Artist enrichment is capped at 40 unique artists; audio features are not fetched.

## Architecture
- index.html: dashboard, CSV parser, core analytics and navigation.
- analytics.js: artwork and diversity insights.
- spotify.js: authentication and API import.
- features.js: sharing and exploration.
- intelligence.js: network, DNA, snapshots, builder and reports.

## Browser tests
Run `npm install`, `npx playwright install chromium`, then `npm test`. Tests cover demo rendering, About navigation, mobile width, intelligence views, Wrapped, CSV import, builder filters and local history. Live Spotify authentication and downloads require separate manual checks. Test execution has not yet been verified.

## Privacy and limits
No backend or automatic tracking. CSV files are processed locally; opt-in snapshots persist in browser storage (up to 50). The collection is session-local. Discovery is search-based, not a recommendation model. TrackSpotify is independent and not endorsed by Spotify.

## Founder
Faris — Founder of TrackSpotify. Contact: farisham10@gmail.com.
