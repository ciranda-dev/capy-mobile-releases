# Capy for Android and iOS

Peer-to-peer meeting rooms on your phone: private calls, notes made on your own device, no accounts and no servers that can read them.

**Releases:** https://github.com/ciranda-dev/capy-mobile-releases/releases · **What's new:** [CHANGELOG.md](CHANGELOG.md) · **Desktop:** https://capy.ciranda.dev/downloads

| Platform | How to get it | Status |
| --- | --- | --- |
| Android (arm64, Android 10 or later) | `Capy-<version>-android-arm64.apk` on the [Releases](https://github.com/ciranda-dev/capy-mobile-releases/releases) page | Beta |
| iOS | TestFlight, by invitation | Beta |

## Install on Android

1. Download the `.apk` of the latest release on your phone.
2. Open it. Android asks you to allow installing apps from the app you opened it with (your browser, Files, Drive…): allow it.
3. Tap **Install**. If Play Protect says the app is unknown, tap **Install anyway**.

**Updating:** install the new `.apk` over the one you have. Don't uninstall first: uninstalling removes what Capy keeps on the phone.

## Verify the download

Each file on a release page shows its SHA-256. To check the file you downloaded, run on a computer:

```sh
shasum -a 256 Capy-<version>-android-arm64.apk     # macOS and Linux (or: openssl sha256 <file>)
certutil -hashfile Capy-<version>-android-arm64.apk SHA256   # Windows
```

and compare it with the one on the release page.

## Report a bug

- In the app: Settings → Help & feedback → Report a bug
- Or open an [issue](https://github.com/ciranda-dev/capy-mobile-releases/issues): what you did, what you expected, what happened, your phone and its system version, and the Capy version (Settings → About)

## Other languages

**Português:** Baixe o `.apk` mais recente na página de [releases](https://github.com/ciranda-dev/capy-mobile-releases/releases) e instale por cima do que você já tem, sem desinstalar. O que mudou está no [CHANGELOG](CHANGELOG.md).

**Español:** Descarga el `.apk` más reciente en la página de [releases](https://github.com/ciranda-dev/capy-mobile-releases/releases) e instálalo encima del que ya tienes, sin desinstalarlo. Lo que cambió está en el [CHANGELOG](CHANGELOG.md).

**العربية:** نزّل أحدث ملف `.apk` من صفحة [الإصدارات](https://github.com/ciranda-dev/capy-mobile-releases/releases) وثبّته فوق النسخة الموجودة دون إزالتها. ما تغيّر موجود في [سجل التغييرات](CHANGELOG.md).

---

Capy is proprietary software, © 2026 Ciranda.
