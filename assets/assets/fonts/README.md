# Bundled font assets

Place the required Noto Sans font files in this directory so the app can load
all glyphs without fetching fonts at runtime. The startup logic expects the
following files:

- `NotoSans-Regular.ttf`
- `NotoSans-SemiBold.ttf`
- `NotoSans-Bold.ttf`

After copying the files, run `flutter pub get` to update the asset manifest. On
startup the app will automatically register the bundled fonts and disable
runtime fetching. If the files are missing, the app falls back to downloading
the fonts at runtime.
