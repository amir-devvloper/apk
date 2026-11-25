# Chamran Admin App (Flutter)

Android admin panel for Chamran car wash.

## What it includes
- Admin login (username: `admin`, password: `chamran1.2.3.4`)
- Orders list (reads local stored orders)
- Manual price entry per order (save turns into edit)
- Financial report (weekly/monthly/yearly) based on entered prices
- Local storage on device

## Build APK with GitHub Actions (cheapest, no local Flutter install)
1. Create a free GitHub account.
2. Create a new repository and upload this `chamran_admin_app` folder contents (the repo root should contain `pubspec.yaml`, `lib/`, `android/`, `.github/`).
3. On GitHub, open **Actions** tab.
4. Run **Build Android APK** workflow (or push to `main`).
5. When it finishes, open the workflow run and download **chamran-admin-apk** artifact.
6. Transfer `app-release.apk` to your Android phone and install it.
   - You may need to allow “Install unknown apps” for your file manager/browser.

## Notes
- This is a Flutter source project. I could not compile the APK in this environment because Flutter/Android SDK are not installed here.
- The workflow uses GitHub-hosted runners to build the APK in the cloud.
