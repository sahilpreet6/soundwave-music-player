# ADR-01: Navigation Strategy

Status: Accepted

## Context

The SoundWave Music Player includes the following main screens:
- Home
- Library
- Playlists
- Settings
- Now Playing screen

The app requires smooth navigation between browsing music and controlling playback. The navigation structure must be simple, clear, and scalable for future updates.

## Decision

The app will use Bottom Tab Navigation for the main sections (Home, Library, Playlists, Settings) and Stack Navigation within each tab for screens such as Song Details, Playlist Details, and Now Playing.

A persistent Mini Player will be displayed at the bottom of the screen, which can expand into a full Now Playing screen.

## Rationale

This navigation structure is commonly used in music applications. It keeps the app organized and easy to understand for users. It also fits the team’s current skill level and reduces the risk of architectural issues during development.

## Consequences

Positive:
- Clear and intuitive navigation
- Easy to expand in future phases
- Organized screen structure

Negative:
- Slight complexity due to nested navigation
