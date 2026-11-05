# Tom Ferry — Trinity Rule (v2.4)
Monthly budget app: Obligations 33% · Investment 33% · Personal 33% · Sadaqat 1%.
Built with HTML/CSS/JS + Capacitor 6, APK built by GitHub Actions.
Dev<Fadhel Abdulla>

## Build
Push to `main` → Actions → download `TomFerry-APK`.

## Stable signing (so updates install over the old version)
```
keytool -genkeypair -v -keystore debug.keystore -alias androiddebugkey -storepass android -keypass android -keyalg RSA -keysize 2048 -validity 10000 -dname "CN=Android Debug,O=Android,C=US"
base64 -w0 debug.keystore
```
Save the output as repository secret `DEBUG_KEYSTORE_B64` (Settings → Secrets and variables → Actions).
