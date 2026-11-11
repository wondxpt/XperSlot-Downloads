# XperSlot — Official Customer and Business apps

**XperSlot is one connected service-booking platform delivered through two independent Android apps.** This repository is the public product-information, release-notes, and download-status hub. Application source code is maintained privately.

<p align="center">
  <a href="https://github.com/wondxpt/Xperslot-Showcase"><img alt="Product overview" src="https://img.shields.io/badge/Product%20Overview-XperSlot-0F766E?style=for-the-badge" /></a>
  <img alt="Apps" src="https://img.shields.io/badge/Apps-Customer%20%2B%20Business-164E63?style=for-the-badge" />
  <img alt="Release status" src="https://img.shields.io/badge/Android%20Release-Preview%20validation-5A55E0?style=for-the-badge" />
</p>

> **Current product line:** XperSlot Customer and XperSlot Business are the two supported app experiences. The former single-app/role-switching concept is not the current product and is not distributed here.

## Choose your app

### XperSlot Customer

A discovery-to-booking experience for customers.

- Discover service businesses and professionals.
- Browse categories, profiles, services, portfolios, and customer feedback.
- Book appointments through business booking pages.
- Manage upcoming and past bookings.
- Save favourites and contact providers through in-app messaging.
- Access a personal profile and customer tools where enabled.

### XperSlot Business

A dedicated workspace for service providers and their teams.

- Set up business details, services, availability, and working hours.
- Manage calendars, appointments, and waitlists.
- Organise staff, shifts, time off, resources, and commissions.
- Maintain client records and customer conversations.
- Access checkout/POS, inventory, reviews, loyalty, gift cards, marketing, and reporting where enabled.

Feature availability depends on account permissions, workspace configuration, and connected services. Both apps require XperSlot online services; neither APK is an offline standalone product.

## Android application identity

| App | Current release candidate | Version code | Android package ID | Minimum Android |
|---|---:|---:|---|---:|
| XperSlot Customer | 2.1.1 | 14 | `com.reservio.customer` | 7.0 / API 24 |
| XperSlot Business | 2.9.5 | 28 | `com.reservio.business` | 7.0 / API 24 |

The package IDs are retained technical identifiers. The built APKs use XperSlot-branded launcher labels.

## Release availability

![Release stage](https://img.shields.io/badge/Release-Preview%20validation-5A55E0?style=for-the-badge)

**No public APK download is available yet.** The Customer 2.1.1 APK is uploaded to the GitHub prerelease draft and GitHub reports the expected full byte size. The Business 2.9.5 APK is still uploading. The draft must remain unpublished until Business is also complete and both assets are independently verified. A draft page is not a public download.

The exact local release-candidate artifacts have been checked:

| Artifact | Size | SHA-256 |
|---|---:|---|
| Customer 2.1.1 (code 14) | 95,546,021 bytes | `0B035AA389129CF10B7E69B82F5DA615C332E7293C94EA7012778ECE801F67D3` |
| Business 2.9.5 (code 28) | 95,546,309 bytes | `1FA233ADF7B7946736261B86BDABC27A95B4F43228E9480199972F8A60FA38E0`

Both candidate APKs passed Android APK Signature Scheme v2 verification. The release certificate SHA-256 is:

```text
5E40400F42768141989602625D157D91C22D0031253D4A766DF2264982874DA2
```

Download and verify the [SHA-256 checksum file](SHA256SUMS.txt) after obtaining the APKs.

## Important installation and upgrade warning

This is intended as the **first public distribution** of XperSlot Customer and XperSlot Business. No earlier public customer installations are being migrated. Some non-public developer test installations were signed with a different certificate:

```text
C2A0EFC0A7A9FB4F8145AE9A4EFF0C0F68386B88D5706F523CF18AA47C95320F
```

Android will reject an in-place update when the installed app and candidate APK have different signing certificates. The different signer affects only those earlier private test installations; Android will reject an in-place update from them. For this first public distribution, use a clean installation. **Do not uninstall a private test installation to force an update**; keep it separate until a migration path is deliberately tested.

## What must be completed before public download

- [x] Verify package IDs, version names, version codes, and minimum Android API from APK metadata.
- [x] Verify APK Signature Scheme v2 and record the signing certificate fingerprint.
- [x] Calculate SHA-256 checksums and compare them with the release checksum record.
- [ ] Upload both APKs and confirm each GitHub asset state is `uploaded` with the expected byte size.
- [ ] Publish the release notes and checksums alongside the two downloadable files.
- [ ] Complete fresh-install smoke tests for both exact public APKs.
- [ ] Document a safe update route for existing installations; never imply signing continuity where it is absent.
- [ ] Validate the key customer and business workflows against the target backend before describing the apps as production-ready.

## Integrity and support

A valid APK signature and matching checksum help detect file changes and identify the signer. They do not prove backend availability, account-flow correctness, booking integrity, or end-to-end production readiness.

- [SHA-256 checksum manifest](SHA256SUMS.txt)
- [Product overview and conceptual architecture](https://github.com/wondxpt/Xperslot-Showcase)
- [Published releases](https://github.com/wondxpt/XperSlot-Downloads/releases)
- [Security policy](SECURITY.md)
- [Support and issue reporting](SUPPORT.md)

For release issues, include the app name, version, Android version, and reproducible steps. Never submit passwords, access tokens, personal data, payment information, or unredacted logs.
