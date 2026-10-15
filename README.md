# INSITE-APK

Android downloads for the FieldTrack student mobile app.

[Download the current APK](https://github.com/jorgencanaveral02-dev/INSITE-APK/raw/refs/heads/main/INSITE.apk)

The `INSITE.apk` file in this repository is version **1.0.0 (Build 44)**.

- Package: `com.fieldtrack.student`
- Default API: `https://insitenc.me/api`
- APK size: 74556061 bytes
- SHA-256: `95571f2e9fd2868c1b0b8bee791e55eee2b2f5fed1f9889451922164335efec9`
- Source revision: `3d5fa3c` in `jorgencanaveral02-dev/INSITE` plus the build number increased from 43 to 44 in `InternShip/pubspec.yaml`.

Build 34 (EDUC student app, attendance): after Time Out or Finish Day, EDUC (BSED/BEED) students see an **E-sign with research teacher** sheet. The student certifies first, then hands the phone to the research teacher on duty, who types a name and position (mobile number optional), accepts a declaration and draws a signature. No teacher account or email is needed. The phone must be at the school, and a signature given after the usual 30-minute window is flagged for the adviser. The Attendance card shows **Waiting for research teacher signature** and **Signed by research teacher**. Build 33 changes remain.

This build needs the matching server update on `https://insitenc.me` (the `esign_pending` and `esign_dtr` attendance actions and the `educ_dtr_esigns` table); without it the E-sign sheet reports an error. The weekly school summary email also needs a public HTTPS `APP_URL` for its report link.

The signing certificate is unchanged from Builds 30 to 33 (SHA-256 b940f541...b68d), so the app updates over the installed one. The E-sign sheet has not been tested on a physical Android phone. The login QR uses the stable download link above, which serves the latest APK committed to this repository. Android may ask you to confirm the download and allow installation from your browser.

Build 36: the document submission confirmation is now a short English line ("I confirm this document is correct, complete, and signed where required."). Same signing certificate as earlier builds, so it updates over the installed app.

Build 37: EDUC students can photograph a signed Notarized Field Study Waiver or Medical Certificate directly (**Already signed? Photograph it now**) without filling in the form first. A saved School ID or other document is no longer reported as "Upload Failed". Same signing certificate as earlier builds, so it updates over the installed app.

Build 38: the Notarized Field Study Waiver accepts one or two photographed pages (Add page / Done), both from Already signed? Photograph it now and after printing it from the app. Same signing certificate as earlier builds, so it updates over the installed app.

Build 39: for EDUC students Time In stays locked on Home and Attendance until the Field Study schedule has started (no schedule yet, or start date still ahead), and says why. Same signing certificate as earlier builds, so it updates over the installed app.

Build 42: rebuilt the current Flutter source. This release process changes only the build number. Package `com.fieldtrack.student`, the default API, and the existing QR download URL are preserved. APK v2 signing was verified with the same certificate as Build 39. The three API-base-URL tests passed. Physical Android installation has not been tested.

Build 43: for CS students all documents are now one list on the **OJT Documents** card, separated by **Print, sign and photograph**, **Upload**, **During OJT** and **After OJT**; the Resume / CV moved into it. CS and HM uploads are no longer shown as being scanned (steps are Uploading, Making sure the file opens, Saving; the result reads **Submission complete**), and the COR/COE of CS/HM is reviewed by staff. This build needs the matching server update on `https://insitenc.me` (the `resume_cv` OJT requirement and the COR/COE manual review); without it the Resume does not appear in the list. Same signing certificate as earlier builds (SHA-256 b940f541...b68d), so it updates over the installed app. Physical Android installation has not been tested.

Build 44: CS students get **DTR Activities** (NC CS OJT Form 4) on the OJT Documents card: log Date / Activities / Hours per day with autosave, print it any time, and photograph the signed copy (one photo per printed page). **DTR Hours** now shows the logged hours as a suggestion when encoding a cutoff. This build needs the matching server update on `https://insitenc.me` (the `dtr_activities` endpoint and catalog row); without it the DTR Activities screen reports an error. Same signing certificate as earlier builds (SHA-256 b940f541...b68d), so it updates over the installed app. Physical Android installation has not been tested.
