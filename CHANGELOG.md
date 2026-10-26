# Changelog

What changed in each release of Capy for Android and iOS. Downloads are on the [Releases](https://github.com/ciranda-dev/capy-mobile-releases/releases) page.

## 0.0.3 · 2026-10-26

- Your 24 words are now sealed by the phone's keychain, kept only on this phone and out of backups; an older install moves them there by itself
- On-device AI on your phone: pick a transcription model (Whisper Tiny, Base or Small) and one to write your notes (Llama 3.2 1B, Qwen3 1.7B or 4B), each saying whether your phone can run it. After a call the minutes, decisions, tasks and chapters write themselves, or tap "Write the notes now". Ask your rooms, and translate captions
- Your voice is transcribed in the language you speak, and short noises no longer turn into words
- Calls ring on your phone while Capy is open, and your own call on another device doesn't ring
- Hold the camera button to record a video message, let go to send, slide away to cancel
- Mic, camera and Leave always stay on screen in a call
- Rooms come back right away when you return to Capy, with a strip saying what Capy is waiting for; messages arrive together instead of one by one
- The chat stays smooth when messages arrive
- A message's time and status sit together at its end; the "+" is inside the message field; photos, room pictures and profile photos open full screen with zoom
- Sending finishes even if you leave Capy right after
- Android: Reply raises the keyboard, and a long-pressed message no longer disappears
- From this version, changes that don't touch the app's native parts arrive over the air

## 0.0.2 · 2026-10-26

- Calls no longer freeze when they open, and buttons answer at once during a call
- The camera opens without a hitch, and calls with video no longer close the app on iPhone
- Transcribing a voice message no longer closes the app on iPhone
- Android: the message field stays above the keyboard, and typing is smoother
- Fixed the "+" menu, the file picker and "Open a saved file", which sometimes did nothing
- Changing the language keeps you on the same page
- Leaving Face ID or a PIN in Lock Capy asks for it first
- Pinned, muted and read rooms follow you from your other devices
- "You're in" no longer comes back at every start
- Your account's files are kept out of phone backups
- Buttons, spacing and the first run's screens redrawn; the recovery words are shown and quizzed in the first run, never copied or saved there
- Add a device: Copy and Share side by side; leaving the screen ends an unused link
- A second always-on relay and blind peer, so people still reach each other when one is down

## 0.0.1 · 2026-10-25

- First test build for Android and iPhone: rooms by invite, messages, voice and video calls, files, the call's notes and the recovery words
- Link a phone to your account from a computer with a QR code or a link; your 24 words stay where they are
- Lock Capy with Face ID, Touch ID, a fingerprint or a PIN
