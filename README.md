# TrackSpotify

A browser-based playlist analytics dashboard. Open index.html or deploy main / (root) with GitHub Pages.

## Data import
Use comma-separated CSV with title and artist columns. Optional fields: album, genre, year, duration_ms, bpm, energy, danceability, valence, acousticness, instrumentalness. Audio features should use 0–1 values. Demo data is fictional; missing audio features are not inferred. Files are processed locally in the browser.

## v0.3
Spotify OAuth with PKCE, permitted playlist import, artwork, artist genre enrichment (up to 40 unique artists per import, subject to API access), diversity and playlist insights. Mood requires imported energy and valence. The GitHub Pages URL is unchanged. Spotify credentials and tokens must never be committed.

## v0.4
Shareable PNG Wrapped card, side-by-side CSV playlist comparisons, Spotify search-based discovery, artist profiles, release-year timeline, session-local imported collection, and clickable artist/genre/decade filters. Collection is limited to manually imported playlists, not listening history. Discovery links are not automated recommendations.

## v0.5
Interactive artist network (top 16 current artists, collaboration and session playlist co-occurrence), heuristic Music DNA, opt-in local playlist snapshots (50 total, unique track changes), current-playlist filter builder with CSV export, and standalone HTML analytics reports. No server, automatic tracking, Spotify playlist write access or new OAuth scopes. CSV history matches by filename-derived playlist name. Live browser tests remain outstanding.
