# ElectroGoniometer - Google Play Data safety notes

These notes are for completing the Play Console form and are not part of the public privacy page.

They reflect the inspected ElectroGoniometer 2.1.1 project. Re-check them against the exact AAB you upload.

## Key distinction

The app accesses and processes measurement, sensor, device, and optional study information locally. In the inspected build, it does not automatically transmit those records off-device to the developer.

User-initiated CSV export/share sends data only to a destination selected by the user. Google Play's Data safety definitions should be applied to the exact behavior of the production build and any included SDKs.

## Current build observations

- No Android `INTERNET` permission in the manifest.
- No developer cloud account or sync feature.
- No ads SDK.
- No analytics SDK.
- No account creation.
- Local SQLite measurement storage.
- Local SharedPreferences for settings.
- Motion/orientation sensor processing.
- Optional study ID, participant ID, and notes entered by the user.
- Device manufacturer/model, OS version, and app version stored with saved measurements.
- CSV export via Android document picker and Android share sheet.
- Individual deletion and delete-all controls.

## Before submitting

Verify every Play Console answer against the signed production AAB. The Play Console Data safety form and public privacy policy must remain consistent.
