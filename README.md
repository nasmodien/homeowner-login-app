# Stitch Hostaway Android App

This is a minimal Android WebView wrapper that loads your Google Stitch export from
`app/src/main/assets/www/stitch_homeowner_login/homeowner_login_1/code.html`.

## Build steps (Android Studio)
1. Open Android Studio → **Open** → select this folder.
2. Let it sync Gradle. If prompted, use JDK 17.
3. Connect a phone (with USB debugging) or start an emulator.
4. **Build > Build Bundle(s) / APK(s) > Build APK(s)**.
5. The APK will appear in `app/build/outputs/apk/debug/` (or `release/`).

## Change the entry screen
Edit `MainActivity.kt` and change the `loadUrl(...)` to another page if desired.

## Network
The app has INTERNET permission. Your pages use `fetch()` against Hostaway.
Remember not to hardcode API keys in production — use a backend proxy if possible.