# BDElectronics Android App

This project is a Capacitor wrapper for [bdelectronics.xyz](https://bdelectronics.xyz).

## Prerequisites
- Node.js (installed)
- Android Studio (required for building APK)

## Project Structure
- `android/`: Contains the native Android project.
- `capacitor.config.json`: Configuration for the app.

## How to Build
1. Open the project in Android Studio:
   ```bash
   npx cap open android
   ```
2. Wait for Gradle sync to complete.
3. To run on a device/emulator: Click the **Run** button (Play icon).
4. To build an APK:
   - Go to **Build > Build Bundle(s) / APK(s) > Build APK(s)**.
   - The APK will be generated in `android/app/build/outputs/apk/debug/`.

## Configuration
To change the website URL, edit `capacitor.config.json`:
```json
{
  "server": {
    "url": "https://your-new-url.com"
  }
}
```
Then run:
```bash
npx cap sync
```
