# INSITE-APK

Android downloads for the FieldTrack student mobile app.

[Download the current APK](https://github.com/jorgencanaveral02-dev/INSITE-APK/raw/refs/heads/main/INSITE.apk)

The `INSITE.apk` file in this repository is version **1.0.0 (Build 47)**.

- Package: `com.fieldtrack.student`
- Default API: `https://insitenc.me/api`
- APK size: 74539949 bytes
- SHA-256: `f568409601e4b2b276a0fc87c59509148a723fc17bb2625f8774d0028342ac0e`
- Source revision: `136f4a4a71549c2642c05dcfa44ddbc13260693a` from the FieldTrack workspace, with the release-only version bump to `1.0.0+47`.

Build 47 (2026-10-20): rebuilt the current student app with self-service **DTR Hours**. Submitted hours count immediately, students can update hours and proof, and the app no longer shows a staff-review waiting state. The matching server update makes Dean and Adviser DTR pages view-only and allows student updates to previously checked cutoffs. Signed proof, placement limits, revision history, and upload-month monitoring are preserved.

Verified: 27 focused DTR/API tests, package and build number, the compiled self-service DTR text, and Android v2 signing with the same certificate as Build 46. The default API and existing QR/download URL are unchanged. Physical Android installation has not been tested.

## Previous builds

Build 46 DTR update (2026-10-20): **DTR Hours** explains that students can submit during a cutoff or after it ends. With the matching server update, CS, HM, and EDUC/COED students can submit ongoing and past cutoffs while keeping the 1-15 / 16-month-end periods, elapsed placement-day limits, signed DTR proof, and Checked locks. The full last cutoff day remains ongoing. Package, API configuration, and signing certificate are unchanged; Android v2 signing and the compiled DTR text were verified. Physical Android installation has not been tested.

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

Version code 2 (2026-10-16): rebuilt from the current Flutter source (medical certificate with several photos, CS Student Information print, signed-capture updates). Same signing certificate as earlier builds (SHA-256 b940f541...b68d). The version code restarted from 44 to 1 in the source, so a phone that still has an old build with a higher version code must uninstall it before installing this one. Physical Android installation has not been tested.

Version code 3 (2026-10-16): **Practicum Updates** and **Weekly Report** add photos from the camera (**Take a photo**) or the gallery (several at once). Photos are straightened, stripped of location data and shrunk before upload, shown in a grid that follows the photo count (1 wide, 2, 3, 2x2, then rows of 3), and can be opened with zoom and removed (Weekly Report also edits the caption there). No server change is needed for the app; the Word export and Dean pages use the same layout once the server has the updated PHP files. Same signing certificate as earlier builds (SHA-256 b940f541...b68d), so it updates over the installed app. Physical Android installation has not been tested.
