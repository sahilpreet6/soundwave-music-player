# ADR-03: Database Storage Strategy

Status: Accepted

## Context

The app needs to store playlists, song metadata, recently played songs, and playback preferences such as shuffle and repeat.

The team considered whether to use a remote backend or local storage.

## Decision

The app will use local storage (unencrypted) for:
- Playlists
- Song metadata
- Recently played songs
- User playback preferences

No remote backend will be used in this phase.

## Rationale

The team has limited experience with backend systems. Using local storage reduces development complexity and allows faster testing. The app does not require handling sensitive user data in this phase.

## Consequences

Positive:
- Simpler implementation
- Works offline
- Easier testing and debugging

Negative:
- No cross-device synchronization
- Limited scalability for future expansion
