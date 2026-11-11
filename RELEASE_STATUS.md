# XperSlot Android release status

**Last checked:** 11 November 2026  
**Current product:** Two independent apps — XperSlot Customer and XperSlot Business  
**Release channel:** GitHub prerelease draft — Customer asset uploaded; Business asset uploading  
**Public download:** Not available until both assets are verified and the draft is published

## Current app identities

| App | Version | Version code | Android package ID | Minimum Android |
|---|---:|---:|---|---:|
| XperSlot Customer | 2.1.1 | 14 | `com.reservio.customer` | API 24 |
| XperSlot Business | 2.9.5 | 28 | `com.reservio.business` | API 24 |

The package identifiers are retained technical IDs. The current product is the separate Customer and Business apps; the former single-app/role-switching concept is not the current product.

## Local release-candidate evidence

The exact release APKs were found in the primary workspace and checked against Android build metadata:

| Check | Customer | Business |
|---|---|---|
| File | `XperSlot-Customer-2.1.1-code14-release-candidate.apk` | `XperSlot-Business-2.9.5-code28-release-candidate.apk` |
| Size | 95,546,021 bytes | 95,546,309 bytes |
| Package | `com.reservio.customer` | `com.reservio.business` |
| Version | 2.1.1 / code 14 | 2.9.5 / code 28 |
| APK Signature Scheme v2 | Pass | Pass |
| SHA-256 | `0B035AA389129CF10B7E69B82F5DA615C332E7293C94EA7012778ECE801F67D3` | `1FA233ADF7B7946736261B86BDABC27A95B4F43228E9480199972F8A60FA38E0` |

The [SHA-256 checksum manifest](SHA256SUMS.txt) is committed in this repository. Both files use release certificate SHA-256:

```text
5E40400F42768141989602625D157D91C22D0031253D4A766DF2264982874DA2
```

The values above describe the local candidate APKs. They do not mean that the files have been uploaded or published.

## GitHub publication status

A prerelease draft was created in this repository:

- Draft release ID: `441034057`
- Draft page: [XperSlot Android Preview](https://github.com/wondxpt/XperSlot-Downloads/releases/tag/untagged-5a4b7739966b129f9bbf)

**Customer is fully uploaded.** GitHub reports asset ID `734970862`, filename `XperSlot-Customer-2.1.1-code14.apk`, exact size `95,546,021` bytes, state `uploaded`, and digest `sha256:0b035aa389129cf10b7e69b82f5da615c332e7293c94ea7012778ece801f67d3`. **Business is still uploading** and has not yet been confirmed as a complete asset. The draft is not a public download page and must remain unpublished until the Business asset is also fully uploaded and verified.

## Signing continuity and installation safety

This is intended as XperSlot's **first public distribution**; no earlier public customer installations are being migrated. Some non-public developer test installations use a different signing certificate:

```text
C2A0EFC0A7A9FB4F8145AE9A4EFF0C0F68386B88D5706F523CF18AA47C95320F
```

The Android package IDs match, but the signing certificates do not. Android will reject an in-place update from those installed builds to these candidates. Those private test installations are not upgrade targets. For the first public distribution, use a clean install; do not uninstall or overwrite a private test installation just to test compatibility.

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
| Existing private-test upgrade | Different signer; not a supported upgrade target | Not applicable to first public distribution |
| Core workflows | Sign-in, customer booking, business calendar, and backend-connected checks on exact release binaries | Pending |
| Production approval | Confirm signing key, version-code history, backend readiness, and operational support | Pending |

## Publication rule

Do not mark the apps as publicly downloadable or production-ready until both APK assets are fully uploaded and the remaining release gates are either passed or clearly documented as limitations. A draft Release, a valid signature, or a successful build is not equivalent to a completed public launch.

For the product scope and app descriptions, see the [XperSlot overview](https://github.com/wondxpt/Xperslot-Showcase). For current download availability, see the [GitHub Releases page](https://github.com/wondxpt/XperSlot-Downloads/releases).
