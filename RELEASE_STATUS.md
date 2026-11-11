# XperSlot Android release status

**Last checked:** 11 November 2026  
**Current product:** Two independent apps — XperSlot Customer and XperSlot Business  
**Release channel:** GitHub prerelease draft in preparation  
**Public download:** Not available yet

## Current app identities

| App | Version | Version code | Android package ID | Minimum Android |
|---|---:|---:|---|---:|
| XperSlot Customer | 2.1 | 13 | `com.reservio.customer` | API 24 |
| XperSlot Business | 2.9.4 | 27 | `com.reservio.business` | API 24 |

The package identifiers are retained technical IDs. The current product is the separate Customer and Business apps; the former single-app/role-switching concept is not the current product.

## Local release-candidate evidence

The exact release APKs were found in the primary workspace and checked against Android build metadata:

| Check | Customer | Business |
|---|---|---|
| File | `app-customer-release.apk` | `app-business-release.apk` |
| Size | 95,590,382 bytes | 95,591,538 bytes |
| Package | `com.reservio.customer` | `com.reservio.business` |
| Version | 2.1 / code 13 | 2.9.4 / code 27 |
| APK Signature Scheme v2 | Pass | Pass |
| SHA-256 | `96577FB1161C26217B1309651D97552EA986448F68702E03743D1C7F8D31EA9E` | `80E1047D2D574BA952E7AC6B644596FB4528BAC396D6650B35ACC320F975DAA1` |

Both files use release certificate SHA-256:

```text
5E40400F42768141989602625D157D91C22D0031253D4A766DF2264982874DA2
```

The values above describe the local candidate APKs. They do not mean that the files have been uploaded or published.

## GitHub publication status

A prerelease draft was created in this repository:

- Draft release ID: `441034057`
- Tag: `xperslot-android-preview-2026.11.11`
- Draft URL: [XperSlot Android Preview](https://github.com/wondxpt/XperSlot-Downloads/releases/tag/untagged-5a4b7739966b129f9bbf)

**The draft currently has no confirmed APK assets. It is not a public download page.** The release must remain a draft until both files are attached and GitHub confirms the full upload state and exact byte sizes.

## Signing continuity and installation safety

Existing protected test installations use a different signing certificate:

```text
C2A0EFC0A7A9FB4F8145AE9A4EFF0C0F68386B88D5706F523CF18AA47C95320F
```

The Android package IDs match, but the signing certificates do not. Android will reject an in-place update from those installed builds to these candidates. The existing apps and their data must not be uninstalled or overwritten as part of this release task.

This is a release candidate for controlled fresh-install evaluation only. No general upgrade compatibility is claimed. Before production distribution, the project must confirm the intended signing key, version-code policy, and supported migration path.

## Release gates

| Gate | Evidence / requirement | Status |
|---|---|---|
| Customer APK build | Release APK exists and metadata matches | Verified locally |
| Business APK build | Release APK exists and metadata matches | Verified locally |
| APK integrity | SHA-256 matches the checked checksum record | Verified locally |
| APK signer | Both pass V2; same release certificate | Verified locally |
| GitHub asset upload | Both asset states must be `uploaded` and sizes exact | Pending |
| Public download links | Both assets must be downloadable by an unauthenticated user | Pending |
| Fresh installation | Install and launch each exact public APK on a clean supported device | Pending |
| Existing-install upgrade | Must not be claimed; current test signer mismatch is confirmed | Blocked |
| Core workflows | Sign-in, customer booking, business calendar, and backend-connected checks on exact release binaries | Pending |
| Production approval | Confirm signing key, version-code history, backend readiness, and operational support | Pending |

## Publication rule

Do not mark the apps as publicly downloadable or production-ready until both APK assets are fully uploaded and the remaining release gates are either passed or clearly documented as limitations. A draft Release, a valid signature, or a successful build is not equivalent to a completed public launch.

For the product scope and app descriptions, see the [XperSlot overview](https://github.com/wondxpt/Xperslot-Showcase). For current download availability, see the [GitHub Releases page](https://github.com/wondxpt/XperSlot-Downloads/releases).
