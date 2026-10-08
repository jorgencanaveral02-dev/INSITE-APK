# INSITE-APK

Android downloads for the FieldTrack student mobile app.

[Download the current APK](https://github.com/jorgencanaveral02-dev/INSITE-APK/raw/refs/heads/main/INSITE.apk)

The `INSITE.apk` file in this repository is version **1.0.0 (Build 36)**.

- Package: `com.fieldtrack.student`
- Default API: `https://insitenc.me/api`
- APK size: 77775886 bytes
- SHA-256: `c49362df32333081d5fa789b0bcf752e14f8c0aa205a389dbbd839df265f14d0`
- Source revision: `95b15eb64bdf3d6fa1127dc709de8ae483428a37` in `jorgencanaveral02-dev/INSITE` plus uncommitted working-tree changes, with the build number increased from 33 to 34.

Build 34 (EDUC student app, attendance): after Time Out or Finish Day, EDUC (BSED/BEED) students see an **E-sign with research teacher** sheet. The student certifies first, then hands the phone to the research teacher on duty, who types a name and position (mobile number optional), accepts a declaration and draws a signature. No teacher account or email is needed. The phone must be at the school, and a signature given after the usual 30-minute window is flagged for the adviser. The Attendance card shows **Waiting for research teacher signature** and **Signed by research teacher**. Build 33 changes remain.

This build needs the matching server update on `https://insitenc.me` (the `esign_pending` and `esign_dtr` attendance actions and the `educ_dtr_esigns` table); without it the E-sign sheet reports an error. The weekly school summary email also needs a public HTTPS `APP_URL` for its report link.

The signing certificate is unchanged from Builds 30 to 33 (SHA-256 b940f541...b68d), so the app updates over the installed one. The E-sign sheet has not been tested on a physical Android phone. The login QR uses the stable download link above, which serves the latest APK committed to this repository. Android may ask you to confirm the download and allow installation from your browser.

Build 36: the document submission confirmation is now a short English line ("I confirm this document is correct, complete, and signed where required."). Same signing certificate as earlier builds, so it updates over the installed app.
