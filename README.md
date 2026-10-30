# One TV — GitHub Actions Android Project

One TV is a separate Android live-TV project for **USHA IT**. It does not share code, package names, databases, or configuration with the earlier Cricket Live project.

## Build without Android Studio

1. Create a GitHub repository.
2. Upload the contents of this folder to the repository root.
3. Open **Actions → Build One TV APK**.
4. Click **Run workflow**.
5. Download the **OneTV-debug-apk** artifact.

The workflow installs JDK 17, Android SDK 36, Gradle 8.13 and builds `app-debug.apk` in GitHub's cloud runner.

## Ads

The project includes the current Unity LevelPlay Android SDK integration and a dedicated Home-page ad section. The app key/ad-unit values should be supplied from the One TV LevelPlay dashboard; do not reuse an ad unit belonging to another app unless it is explicitly configured for One TV.

## Streams

The included streams are public demo streams used only to validate playback. Replace them with official/authorized TV streams before publishing. The project is intentionally not bundled with scraped/private IPTV sources.

## Planned production architecture

`Admin Panel → API/Backend → Database → One TV Android App`

Channel URLs, names, logos, categories and status should be managed from the backend so stream changes do not require an APK update.

## Branding

`© 2026 USHA IT. All Rights Reserved.`
