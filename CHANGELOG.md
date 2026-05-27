# Changelog

All notable changes to AI GOD (direct edition) are documented here.

## [1.0.5] - 2026-05-26

### Fixed
- Prevented an unhandled JavaScript error after granting microphone access
  on macOS 26.5 (Tahoe). All microphone-related calls now degrade gracefully
  to console.warn instead of disrupting the UI.
- Registered missing IPC stubs (aigod:license-status, aigod:license-activate)
  in the Mac App Store build so the renderer initializes cleanly on first launch.

### Added
- NSMicrophoneUsageDescription in Info.plist for both MAS and Developer ID
  builds (required on macOS 14+).
- Global error safety net in the renderer: unhandled errors and rejected
  promises are now caught silently and logged to the console.

## [1.0.4] - 2026-05-25

### Fixed
- MAS-only crash on launch caused by a missing IPC handler for
  aigod:license-status.

## [1.0.3] - 2026-05-15

### Changed
- Internal Express backend now binds to 127.0.0.1 (loopback) instead of
  0.0.0.0. The app no longer requests com.apple.security.network.server.
- Removed unused entitlements: application-groups, device.camera,
  automation.apple-events.

## [1.0.2] - 2026-05-14

### Added
- Price string updated to 29.99 EUR across all 6 languages.

### Fixed
- File picker filename label now localizes correctly when language changes.

## [1.0.1] - 2026-05-12

### Fixed
- First Apple Review feedback: clearer error messages and localized error text.
- Portuguese added to the native macOS application menu.

## [1.0.0] - 2026-05-05

Initial public release.

- Native macOS Electron app, universal binary (Apple Silicon + Intel).
- 4 AI providers: OpenAI, Anthropic, Google, OpenRouter.
- Voice in (Whisper) and voice out (OpenAI TTS).
- Image generation (DALL-E / GPT Image 1).
- 6 languages: EN, ES, FR, DE, IT, PT.
- 15-day free trial + Ed25519 offline lifetime license.
