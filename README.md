# Aether Study Hub — Android app wrapper

This Android Studio project packages the supplied Aether Study Hub web app in an Android WebView. App data is stored by the web app in the app's local browser storage. Internet is used for the Google Fonts and Chart.js CDN and for embedded media; the core HTML is bundled in the APK.

## Build an APK with GitHub Actions (phone-friendly workflow)
1. Create a GitHub repository and upload the contents of this folder (not the outer ZIP) to the repository's main branch.
2. Open the repository's **Actions** tab. If prompted, enable Actions.
3. Choose **Build Android APK** → **Run workflow**.
4. When it finishes, open the run and download the **Aether-Study-Hub-APK** artifact. Extract the ZIP to get `app-debug.apk`.
5. Transfer `app-debug.apk` to your Android phone and open it. Android may ask you to allow installs from that file app; only allow it for this APK if you trust the source.

## Build on a computer
Open this folder in Android Studio and build/run the `app` module, or run `gradle assembleDebug` with Java 17, Android SDK platform 35, and Android build tools installed.

The debug APK is for personal testing, not Play Store publication. Keep the source and repository private if you don't want the app code public.
