# INSITE-APK

Android downloads for the FieldTrack student mobile app.

[Download the current APK](https://github.com/jorgencanaveral02-dev/INSITE-APK/raw/refs/heads/main/INSITE.apk)

The `INSITE.apk` file in this repository is version **1.0.0 (Build 33)**.

- Package: `com.fieldtrack.student`
- Default API: `https://insitenc.me/api`
- APK size: 77661126 bytes
- SHA-256: `dd9609245c6df390a085b27d9fd868f20bccce4f4c2c0fe106348b3043ad5ecb`
- Source revision: `84cbf6bd4f31b59cb1876eb1ba355dd2f5bbeecd` in `jorgencanaveral02-dev/INSITE` plus uncommitted working-tree changes, with the build number increased from 32 to 33.

Build 33 (EDUC student app, Case Study): a saved Case Study now shows **Awaiting signed copy** until the student prints it, has it signed by the Resource/Cooperating Teacher and uses **Capture signed copy** to photograph every signed page (1 to 5 pages, merged into one PDF tied to that exact report and version). The statuses are Awaiting signed copy, For review, Approved and Returned for correction; **Late** is a separate marker. Approved reports are locked, a returned report shows the reviewer's feedback and can be recaptured or corrected (a changed report needs a new print, signature and capture), and the Case Study list has a month selector. The printed copy carries "Case Study #id - version N" in its footer. Both the Dean and the Adviser can review.

This build needs the matching server update (new `student/case_study_signed_copy.php` endpoint and Case Study schema) on `https://insitenc.me`; without it the capture button reports an error. Build 32 changes remain.

The signing certificate is unchanged from Builds 30 to 32 (SHA-256 b940f541...b68d), so the app updates over the installed one. Camera capture and printing have not been tested on a physical Android phone. The login QR uses the stable download link above, which serves the latest APK committed to this repository. Android may ask you to confirm the download and allow installation from your browser.
