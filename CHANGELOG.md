# Changelog

What changed in each release of Capy for Android and iOS. Downloads are on the [Releases](https://github.com/ciranda-dev/capy-mobile-releases/releases) page.

## 0.0.11 · 2026-11-05

- Edit a message: long-press it and pick Edit. It says "Edited", and someone on an older Capy keeps seeing the first text
- Polls in a room, find a time and approving a call's minutes, the same as on the desktop. Votes are open and named: everyone in the room, now and later, sees who voted for what
- Translate a message on this phone with the captions' translation models. Code, links and mentions stay as written, and nothing is sent
- Handset mode: hold the phone to your ear in a voice call and the sound moves to the earpiece and the screen turns off. Turn it off in Settings → Audio & video
- Present a PDF in a call on Android, read in a worker of its own. iPhones can't yet: the iPhone's JavaScript engine in Capy has no WebAssembly
- This version has new code inside the app, so it does not come over the air: install the APK or TestFlight build 11

## 0.0.10 · 2026-11-04

- Background in calls: blur what's behind you (light or strong) or put a picture there (four come with Capy, or up to three of your own, kept on this phone and removed by Log out and erase). It's worked out on the phone before the camera goes out; if the phone can't keep up or gets too hot, your camera goes off for the others rather than send the room as it is. Pick it in the call's lobby, in the call's More menu, or in Settings → Audio & video. Photos and video messages go as the camera sees them
- On iPhone the effect uses Apple's Vision, on Android MediaPipe's Selfie Segmentation. Nothing is downloaded and nothing is sent anywhere for it
- This version has new code inside the app, so it does not come over the air: install the APK or TestFlight build 10

## 0.0.9 · 2026-11-03

- Switching tabs in the emoji picker (Emoji, Capy, Stickers, GIFs) no longer closes the app

## 0.0.8 · 2026-11-02 (0.0.5 to 0.0.7 went out over the air with it)

- A notification for every message: each message you send, a text, a photo, a file, a voice or video message, now wakes the room's members who aren't connected, on their iPhone, with a notification of its own, at most one a second for each room. Before, a burst of messages made one notification, and a voice message, a photo or a file sent soon after a text made none
- On iPhone, notifications with Capy closed come through the team's push gateway, with nothing readable going through Apple or Google (they see that a push came for a code that names nothing, and when; never what, who or which room), and each one of a room's new messages adds one to the number on Capy's icon. Both need TestFlight build 7 or later
- On Android, the icon's dot and number follow Capy's notifications, and Stay connected in the background now really keeps Capy connected behind other apps (0.0.4 paused it, so nothing came). Settings → Notifications says what to set when your phone's battery manager stops Capy anyway, with a button to Capy's app info
- A ringing call vibrates, twice each time the ringtone loops, and pulses around the room's picture while Capy is on screen. Busy rings silently, and Capy's Do not disturb doesn't ring
- A call you start reaches at once a member whose connection had dropped, instead of minutes later or not at all
- Swipe to reply works under a finger, on iPhone and Android; on iOS 26 the chat no longer slides back to your rooms instead
- Choosing Reply scrolls the chat to its newest message, in a room and in a thread, and tapping a quoted message glides there and lights it up for a moment
- When nobody who runs a room but the person you're reporting can receive a report, the report now says to ask the owner to name an admin

## 0.0.4 · 2026-11-01

- A shorter first run: say hello, pick your name and you're in. Once you have a room, a card asks you to save your 24 words, then or later; locking Capy and adding a device come up the same way
- The app icon shows how many messages wait for you (secure rooms are never counted)
- Swipe anywhere on a message to the right to reply
- A held video message stops into a review (play it, then Send, Record again or Discard), as voice messages do
- Only the ticks beside a message's time: one sent, two delivered, two in colour seen
- The message field goes back to its size after you send a long message
- A voice or video message, or a file, says "Sending…" until it is kept for the room, so the others can get it while you're offline
- In a call, your own other devices show as tiles, with what they share or present
- Logging out covers the app until it's done
- The notes model no longer closes the app on a phone without the memory for it: one model runs at a time, and the notes say why when one couldn't
- Block someone from their card; Settings → Privacy & security → Blocked people lists them
- The "Words locked" screen no longer sends you back to itself
- Capy uses the team's new relay, files and video messages go up to 10 MB like on computers, and the voice filter is gone
- Messages and calls reach you with Capy closed. On iPhone through Holepunch's blind-push (Apple and Google see that a notification came, never what, who or which room; the phone writes the words itself). On Android, Capy stays connected in the background, with no Google service at all. Both are on by default, in Settings → Notifications
- Report a message or a person to the room's owner and admins (sealed to them), and see a room's reports if you run it
- Share your phone's screen in a call, from More: the others see it as they see a computer's, and it turns with your phone. Never in a secure room
- Smoother video: the people in a call are drawn at the frame rate they send (before, a computer's 24 a second showed as 12), your own preview runs at the camera's best rate, and your tile no longer goes blank when the call's panel opens
- Two people in a call who couldn't reach each other at first now connect by themselves
- This version needs the new app from the store or the APK: 0.0.3 doesn't take it over the air

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
