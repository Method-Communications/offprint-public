# offprint-public

Distribution files for **Offprint**, an internally built Chrome extension used at
Method Communications. This repository exists for one reason: Chrome fetches an
extension and its update manifest anonymously, so those two files have to sit
somewhere publicly readable.

**There is no source code here.** Just the signed bundle and the manifest Chrome
polls:

| File | What it is |
|---|---|
| `offprint-1.2.0.crx` | the signed extension |
| `update.xml` | Chrome update manifest |

## What Offprint does

Turns an article page into a clean reading view: title, byline, body text and
images, on a plain background, with a light/dark toggle and a print button.

It runs entirely on the device. It requests three permissions (`activeTab`,
`scripting`, `storage`), makes no network requests of its own, and contains no
analytics or telemetry of any kind. Chrome shows no permission warning for it,
which you can verify yourself: unzip the `.crx` and read `manifest.json`.

## Third-party code

Mozilla Readability 0.6.0, vendored unmodified, **Apache License 2.0**. The
licence text and full attribution ship inside the bundle at
`vendor/readability-LICENSE.md` and `THIRD_PARTY_NOTICES.md`.

## Scope

Published for distribution to Method-managed devices. Not intended for general
use, and offered without support or warranty. If you found this looking for a
reader extension, Firefox has Reader View built in.
