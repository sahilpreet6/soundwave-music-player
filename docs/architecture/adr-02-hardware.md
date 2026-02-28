# ADR-02: Hardware Integration

Status: Accepted

## Context

The SoundWave Music Player requires audio playback functionality. The app must support music playback even when running in the background.

Advanced hardware features such as GPS or biometric authentication are not required for this project.

## Decision

The app will use:
- Device speaker/audio output
- Background audio playback
- Lock screen and notification controls
- Bluetooth audio support

The app will not use:
- GPS
- Fingerprint or Face ID
- Camera

## Rationale

The focus of this phase is stable and reliable playback functionality. Adding unrelated hardware features would increase complexity and risk within the project timeline. Only essential audio-related hardware features will be implemented.

## Consequences

Positive:
- Complete music playback experience
- Realistic app behavior
- Reduced development risk

Negative:
- Limited advanced features in early phases
