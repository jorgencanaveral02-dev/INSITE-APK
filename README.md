# INSITE-APK

Android downloads for the FieldTrack student mobile app.

- [Download the latest APK](https://github.com/jorgencanaveral02-dev/INSITE-APK/releases/latest/download/INSITE.apk)
- [View the current release](https://github.com/jorgencanaveral02-dev/INSITE-APK/releases/latest)

The `INSITE.apk` file in this repository is version 1.0.7 (build 15).

Default API: `https://insitenc.me/api`

SHA-256: `A2DB14D61ACC8291A13525AE0D864464B7BE1C6953A0CFD457BAD2AAC4E5B567`

Includes the CS/HM Pre-Deployment and Deployment Clearance flow plus the DEMO upload fix:

- Pre-Deployment shows the full applicable starting checklist and document actions.
- Deployment Clearance shows final readiness, approvals, pending reasons, and the official start date.
- Existing MOA and endorsement approval prerequisites remain enforced.
- COED keeps its existing workflow.
- The app confirms the selected MOA or Acceptance filename before uploading.
- DEMO-marked files on real accounts are checked separately from official submissions.
- Superseded demo documents no longer appear as the current MOA.

Source: [a90f8b1](https://github.com/jorgencanaveral02-dev/INSITE/commit/a90f8b1ba766b830db7c95cc181ec22aabec4ffc).

Verified with PHP syntax checks, Flutter analysis, five mobile flow tests, a release APK build, and signing-certificate continuity with build 14. Actual phone behavior has not been tested.
