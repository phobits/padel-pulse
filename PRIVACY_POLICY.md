# Privacy Policy

**Point-Counter** (Android) and **Padel Pulse** (iOS) are free, open-source scoreboard applications. Both apps apply the same zero-data-collection guarantee described below.

## Data Collection

Neither app collects, stores, or transmits any personal data. Specifically:

- No user accounts or login required
- No analytics or tracking
- No internet connection required or used
- No data is sent to any server
- No cookies or remote storage of personal information
- Bluetooth is used only for receiving button presses from paired HID / media-remote devices — no data is transmitted

Match history and in-progress match state are stored only on-device (SharedPreferences on Android, UserDefaults on iOS) and are removed when the app is uninstalled.

## Permissions

### Android (Point-Counter)

- **Camera**: Used solely for recording games on-device. Video recordings are stored locally on your device and are never uploaded or shared by the app.
- **Bluetooth**: HID devices work through standard Android system pairing without any app-level Bluetooth permissions.

### iOS (Padel Pulse)

- **Camera** (`NSCameraUsageDescription`): Optional. Only accessed when the camera overlay is explicitly enabled in Settings and the user opens the on-court camera preview. Nothing is captured without that user action.
- **Microphone** (`NSMicrophoneUsageDescription`): Optional, tied to Camera. Active only while a video clip is being recorded so the clip has its ambient audio.
- **Photo Library — Add Only** (`NSPhotoLibraryAddUsageDescription`): Optional. Only used to save a finished video clip to the user's Photos library. The app requests write-only access (`PHAccessLevel.addOnly`) — it cannot read existing photos.
- **Bluetooth remotes**: Handled via the system-wide `MPRemoteCommandCenter` (Next Track, Previous Track, Play/Pause). Uses standard iOS media-control APIs — no dedicated Bluetooth permission is required and no data is transmitted.
- **No location, no contacts, no calendar, no tracking identifiers** are requested.

If Camera, Microphone, or Photo Library permissions are denied, the app continues to function for scoring — only the opt-in recording feature is disabled.

## Third-Party Services

Neither app uses third-party services, SDKs, or libraries that collect data.

## Changes

If this policy changes, updates will be posted in this file in the app's source repository.

## Contact

If you have questions about this privacy policy, please open an issue on the relevant repository:

- Android: [github.com/DominikLindorfer/Point-Counter](https://github.com/DominikLindorfer/Point-Counter)
- iOS: [github.com/phobits/padel-pulse](https://github.com/phobits/padel-pulse)

*Last updated: April 2026*
