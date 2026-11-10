# XperSlot — Two Apps. One Connected Booking Experience.

XperSlot is a service-booking platform built around two dedicated experiences: **XperSlot Customer** for people discovering and booking services, and **XperSlot Business** for the professionals and teams delivering them.

This repository is the public download hub. The application source repository remains separate and private.

## Choose your app

### XperSlot Customer

A discovery-to-booking experience for customers.

- Explore service businesses and professionals.
- Search and browse by business category, with map-based discovery.
- Review business profiles, portfolios and customer feedback.
- Book appointments through business booking pages.
- Keep upcoming and past bookings together.
- Save favourite businesses and contact providers through in-app messaging.
- Access a personal profile, wallet, support and customer forms.

### XperSlot Business

A workspace for service businesses and their teams.

- Set up a business workspace and manage business details.
- Manage the service catalogue, availability, working hours and booking rules.
- Work with a business calendar, appointments and waitlists.
- Organise staff, shifts, time off, resources and commissions.
- Maintain client records and communicate with customers.
- Track payments, checkout/POS, inventory and store orders.
- Manage reviews, gift cards, loyalty, discounts and marketing tools.
- Review business activity and reporting, and manage online presence.

Feature access can vary by account role, workspace configuration and connected services. The apps require the XperSlot backend and account services; an APK alone is not a standalone offline product.

## Android preview builds

The current public Android package is a **preview / release-candidate build**, not a declaration that every production rollout and store-signing prerequisite has been completed.

| App | App version | Android version code | Minimum Android | Package ID |
|---|---:|---:|---:|---|
| Customer | 2.1 | 13 | Android 7.0 (API 24) | com.reservio.customer |
| Business | 2.9.4 | 27 | Android 7.0 (API 24) | com.reservio.business |

The legacy Android package identifiers are intentionally retained in these builds. The launcher labels identify the apps as **Xperslot Customer** and **Xperslot Business**.

**Get the APKs:** open the [Android preview release](https://github.com/wondxpt/XperSlot-Downloads/releases/tag/android-preview-2026.11.10) and download the APK for the audience you belong to.

## Installation and upgrade notes

1. Download only the APK for your intended app: Customer or Business.
2. Open the downloaded APK on an Android device and follow Android's installation prompt.
3. Sign in or create an account, then use the app with a supported network connection.

These preview APKs are signed and their APK Signature Scheme v2 signatures verify. However, the release signing key has not yet been confirmed against every previously distributed production build. Existing debug-signed test installations may reject an in-place update. **Do not uninstall an existing installation just to try this preview**: uninstalling can remove local app data. Wait for a signing-key and upgrade-path confirmation first.

## Integrity and security details

- Both APKs pass Android APK Signature Scheme v2 verification.
- Both variants are configured as non-debuggable release builds.
- Android app backup is disabled, with backup and device-transfer exclusions.
- Cleartext HTTP traffic is disabled in the Android manifest.
- The certificate SHA-256 fingerprint for these preview builds is:

  5E40400F42768141989602625D157D91C22D0031253D4A766DF2264982874DA2

A verified APK signature establishes package integrity and signer identity; it does not by itself prove backend availability, account-flow correctness or compatibility with every previously installed build. Production rollout and end-to-end validation remain separate release gates.

## Feedback

Please use the repository's [Issues](https://github.com/wondxpt/XperSlot-Downloads/issues) for reproducible download or installation problems. Do not include passwords, access tokens, personal data or private account information in an issue.