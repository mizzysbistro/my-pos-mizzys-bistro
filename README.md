# MY POS — Mizzy’s Bistro

Public Android POS project with an editable HTML preview and GitHub Actions APK build.

## Project layout

- `preview/mizzy-bistro-pos-fixed.html` — editable standalone HTML preview.
- `app/src/main/assets/index.html` — HTML loaded by the Android WebView app.
- `app/` — native Android wrapper.
- `.github/workflows/build-apk.yml` — builds a debug APK on every push to `main` and on manual dispatch.

## Build APK

Open **Actions → Build MY POS APK → Run workflow**. When successful, download the `my-pos-debug-apk` artifact. The artifact is a debug APK for testing, not a signed production release.

## Notes

The standalone preview and WebView app should stay in sync. Review tax/legal receipt requirements, local printer integration, authentication, backup/sync, and payment-provider integration before production use. Never store secrets in this public repository.
