# ADR-03: Database Storage Strategy

Status: Accepted

## Context

The app needs to store playlists, song metadata, recently played songs, and user playback preferences such as shuffle and repeat.

The team considered whether to use a remote backend or local storage.

## Decision

The app will use local storage (unencrypted) for:
- Playlists
- Song metadata
- Recently played songs
- User playback preferences

No remote backend will be used in Phase 2.

## Rationale

The team has limited experience with backend development. Using local storage reduces complexity and allows faster development and testing. The app does not require handling sensitive user data in this phase.

## Consequences

Positive:
- Simpler implementation
- Works offline
- Faster debugging

Negative:
- No cross-device synchronization
- Limited scalability in early stages
