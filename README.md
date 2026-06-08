# IrisHandheld — OTA release artifacts

Public hosting for **staffV3** Sunmi handheld over-the-air updates.

The device polls `releases/latest/download/staffv3-manifest.json`. To publish a
new build, run `scripts/publish-ota.sh` in the IrisHandheld repo (bump
`app/version.properties` first). No secrets live here — the APK reads the
payment key from device settings, not from the bundle.