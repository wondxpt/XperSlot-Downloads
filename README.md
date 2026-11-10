# XperSlot — Official Customer and Business apps

XperSlot is a service-booking platform with **two separate Android applications**. This repository is the official public product-information and release-status hub. The application source code is maintained separately in a private repository.

<p align="center">
  <a href="https://github.com/wondxpt/Xperslot-Showcase"><img alt="Product overview" src="https://img.shields.io/badge/Product%20Overview-XperSlot-0F766E?style=for-the-badge" /></a>
  <img alt="App model" src="https://img.shields.io/badge/Apps-Customer%20%2B%20Business-164E63?style=for-the-badge" />
  <img alt="Launch" src="https://img.shields.io/badge/Public%20APK%20Release-Coming%20Soon-5A55E0?style=for-the-badge" />
</p>

> **Current product line:** XperSlot Customer and XperSlot Business are the only two apps presented by this project. The earlier single-app/role-switching concept is not the current product and is not offered for download.

## Choose your app

### XperSlot Customer

A discovery-to-booking experience for customers.

- Explore service businesses and professionals.
- Search and browse by business category, including map-based discovery.
- Review business profiles, portfolios, and customer feedback.
- Book appointments through business booking pages.
- Keep upcoming and past bookings together.
- Save favourite businesses and contact providers through in-app messaging.
- Access a personal profile, wallet, support, and customer forms where enabled.

### XperSlot Business

A workspace for service businesses and their teams.

- Set up a business workspace and manage business details.
- Manage services, availability, working hours, and booking rules.
- Work with a business calendar, appointments, and waitlists.
- Organise staff, shifts, time off, resources, and commissions.
- Maintain client records and communicate with customers.
- Manage payments, checkout/POS, inventory, and store orders where enabled.
- Work with reviews, gift cards, loyalty, discounts, and marketing tools.
- Review business activity and reporting, and manage online presence.

Feature access can vary by account role, workspace configuration, and connected services. The apps require XperSlot backend and account services; an APK by itself is not a standalone offline product.

## Android app identity

| App | Android package ID |
|---|---|
| XperSlot Customer | `com.reservio.customer` |
| XperSlot Business | `com.reservio.business` |

The package identifiers are retained technical IDs for application continuity. The user-facing launcher labels identify the two apps as **XperSlot Customer** and **XperSlot Business**.

## Download availability

**There is currently no published XperSlot APK release in this repository.** The incomplete draft release has been removed. This page is the official status page, not an APK download link.

A public release will be created only when:
- Both current APK files are attached and GitHub confirms each upload is complete.
- Package IDs, app labels, version names, version codes, and minimum Android requirements match the actual files.
- SHA-256 checksums are published and verified against the downloadable binaries.
- The signing certificate and in-place upgrade path are checked against previously distributed installations.
- Fresh installation and update behavior are smoke-tested on physical Android devices.
- Core sign-in, customer booking, business calendar, and backend-connected workflows are validated.

Until then, do not install unofficial mirrors or use an old single-app build as a substitute for either current app.

## Installation and upgrade safety

When the public release is available, use only the APK links in the published GitHub Release and follow its version-specific instructions.

Do not uninstall an existing XperSlot installation merely to test a candidate build. Android may reject an update signed with a different certificate, and uninstalling can remove local app data. Wait for the release notes to explicitly confirm the supported update path.

## Integrity and security

A valid Android APK signature helps establish the identity of the signer and detect file modification. It does not by itself prove backend availability, account-flow correctness, booking integrity, or compatibility with an older installation. Those checks are handled separately before release.

For security concerns, see [SECURITY.md](SECURITY.md). For installation or product support, see [SUPPORT.md](SUPPORT.md).

## Feedback

Use [GitHub Issues](https://github.com/wondxpt/XperSlot-Downloads/issues) for reproducible product or release problems and focused feature requests. Do not include passwords, access tokens, personal data, private messages, payment details, or unredacted logs.

- [Product overview and architecture](https://github.com/wondxpt/Xperslot-Showcase)
- [Published releases](https://github.com/wondxpt/XperSlot-Downloads/releases)
