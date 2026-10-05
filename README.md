# INSITE-APK

Android downloads for the FieldTrack student mobile app.

[Download the current APK](https://github.com/jorgencanaveral02-dev/INSITE-APK/raw/refs/heads/main/INSITE.apk)

The `INSITE.apk` file in this repository is version **1.0.0 (Build 26)**.

- Package: `com.fieldtrack.student`
- Default API: `https://insitenc.me/api`
- APK size: 77,067,578 bytes
- SHA-256: `c82404b8f5dd1cd3258ead6895cbffa4a4a1e3bb2cd379951523bc295a6a1981`
- Built from [source 14ae927](https://github.com/jorgencanaveral02-dev/INSITE/commit/14ae927df925860d4c6d389544e2fc0fcc62b1b4).

Rebuilt the current Flutter app and removed an identical duplicate company-profile API declaration that prevented compilation. The existing package, API default, app behavior, and signing certificate are retained.

Verified release compilation, Android v2 signing, signing certificate continuity with Build 25, three API URL tests, service analysis, PHP syntax, and live QR/download routing. Existing merge conflicts and duplicate mock declarations prevent the HTE widget test files from running. Physical Android installation has not been tested.

Opening the login QR starts the APK download directly. Android may ask you to confirm the download and allow installation from your browser.
