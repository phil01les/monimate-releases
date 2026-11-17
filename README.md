# Monimate update channel

update.json plus one APK per release. Public on purpose: the app reads the manifest without
credentials, then downloads the APK it names and checks its SHA-256.

Written only by tools/release_apk.ps1 in the app repository. A hand-edited manifest is how a wrong
hash or a stale versionCode gets shipped, so nothing else should touch these files.