# TrackSpotify

A browser-based playlist analytics dashboard. Open index.html or deploy main / (root) with GitHub Pages.

## Data import
Use comma-separated CSV with title and artist columns. Optional fields: album, genre, year, duration_ms, bpm, energy, danceability, valence, acousticness, instrumentalness. Audio features should use 0–1 values. Demo data is fictional; missing audio features are not inferred. Files are processed locally in the browser.

## v0.3
Spotify OAuth with PKCE, permitted playlist import, artwork, artist genre enrichment (up to 40 unique artists per import, subject to API access), diversity and playlist insights. Mood requires imported energy and valence. The GitHub Pages URL is unchanged. Spotify credentials and tokens must never be committed.
