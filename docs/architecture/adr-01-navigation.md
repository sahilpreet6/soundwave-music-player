# ADR-01: Navigation Strategy

Status: Accepted

## Context

The SoundWave Music Player includes the following main screens:
- Home
- Library
- Playlists
- Settings
- Now Playing screen

Users need to move easily between browsing songs and controlling playback. The navigation must be simple, organized, and easy to expand in later phases.

## Decision

The app will use Bottom Tab Navigation for the main sections (Home, Library, Playlists, Settings). 

Stack Navigation will be used inside each tab for screens such as Song Details, Playlist Details, and the Now Playing screen.

A persistent Mini Player will appear at the bottom of the screen and can expand into a full Now Playing screen.

## Rationale

This structure is commonly used in music applications and is easy for users to understand. It keeps the app organized and allows us to expand features later without redesigning everything. It also matches our team’s current skill level.

## Consequences

Positive:
- Clear and intuitive navigation
- Easy to maintain and expand
- Organized screen hierarchy

Negative:
- Slight complexity due to nested navigation
