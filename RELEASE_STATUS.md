# XperSlot Android release status

**Last checked:** 11 November 2026  
**Current product:** Two separate apps — XperSlot Customer and XperSlot Business  
**Public APK release:** Not yet published

## Current app structure

| App | Android package ID |
|---|---|
| XperSlot Customer | `com.reservio.customer` |
| XperSlot Business | `com.reservio.business` |

The package IDs are technical identifiers retained for application continuity. The current product is the separate Customer and Business apps. The older single-app/role-switching concept is not the current product and must not be presented as the current release.

## Release state

- The incomplete GitHub draft release for the previous candidate was removed.
- No APK download is currently published from this repository.
- A previous physical-device startup check verified installation and launch of the protected Customer and Business app snapshots. That check does not establish end-to-end readiness of the exact binaries intended for public distribution.
- Exact release APKs must be re-verified for package identity, version metadata, signing certificate, file checksum, and upgrade compatibility before upload.
- Existing installations must not be uninstalled merely to test a candidate; update compatibility must be established first.

## Publication gates

| Gate | Required evidence | Status |
|---|---|---|
| Customer APK | Current binary, correct package and version metadata | Pending |
| Business APK | Current binary, correct package and version metadata | Pending |
| Artifact integrity | SHA-256 published and matched to both APKs | Pending |
| Signing continuity | Certificate and supported upgrade path confirmed | Pending |
| Fresh installation | Both apps install and launch on supported Android versions | Pending |
| Existing-install upgrade | Update succeeds without uninstalling or losing local data | Pending |
| Core workflows | Sign-in, customer booking, business calendar, and backend-connected flows checked | Pending |
| Release notes | App versions, package IDs, Android requirements, checksums, and known limitations documented | Pending |

## Publication rule

Do not announce APK downloads until both files are fully uploaded and every release gate above has evidence. A signature check or successful launch alone is not full end-to-end release validation.

The official download location is the [GitHub Releases page](https://github.com/wondxpt/XperSlot-Downloads/releases). Only a published release containing two complete APK attachments is considered downloadable.
