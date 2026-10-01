# XTAK

XTAK is an ATAK 5.5-based Android tactical mapping implementation focused on decentralized, distributed, and resilient field operations.

This repository contains the public source release for XTAK and links to the corresponding release APK.

## Current Public Release

**XTAK 5.5.1.8**

- Release APK: [XTAK-5.5.1.8-c1-civ-release.apk](https://github.com/5lyf0x/XTAK/releases/tag/v5.5.1.8)
- Public source package: [XTAK-5.5-public-release-source.zip](./XTAK-5.5-public-release-source.zip)
- Release tag: [v5.5.1.8](https://github.com/5lyf0x/XTAK/releases/tag/v5.5.1.8)

## About XTAK

XTAK builds on the ATAK CIV 5.5 codebase while exploring capabilities intended for environments where connectivity may be intermittent, infrastructure may be unavailable, and peer-to-peer operation is important.

The project direction includes:

- decentralized and distributed TAK workflows
- resilient peer-to-peer communications
- local and mesh-oriented data exchange
- reduced dependence on centralized infrastructure
- tactical mapping and situational-awareness workflows
- support for extensible field integrations and plugins

XTAK is intended for experimentation, development, interoperability testing, and legitimate operational use by authorized users.

## Downloads

The recommended way to obtain the compiled application is from the GitHub **Releases** page:

[Download XTAK releases](https://github.com/5lyf0x/XTAK/releases)

The current release APK is:

`XTAK-5.5.1.8-c1-civ-release.apk`

For integrity verification, the SHA-256 digest of the current APK is:

```text
c99cce516da0e847314647332b89f639752b32102a90649b67bc6d7530c1feca
```

## Source Code

The corresponding public source package is included in this repository:

`XTAK-5.5-public-release-source.zip`

This archive contains the source associated with the public XTAK 5.5 release.

## Plugins

XTAK includes several companion plugins that extend the base application with additional field capabilities.

> **Development status:** All of the plugins below are still under active development. Each is at least partially functional, but features, compatibility, user interface, and behavior may change between builds.

### XTAK VISION

[XTAK VISION R2-i06.apk](./XTAK%20VISION%20R2-i06.apk)

XTAK VISION is a camera and augmented-reality plugin for displaying nearby TAK objects in the live camera view. It is designed to provide a tactical heads-up view with projected object positions, bearing/distance information, native item details, observation and media capture features, and source-aware highlighting for supported sensor tracks.

### XTAK ADS-B

[XTAK-ADSB-0.1.0-i03-civRelease.apk](./XTAK-ADSB-0.1.0-i03-civRelease.apk)

XTAK ADS-B brings aircraft tracking data into XTAK. It is intended to receive and display ADS-B-derived aircraft positions as live situational-awareness objects on the map for local air-traffic awareness and sensor integration.

### XTAK Voice

[XTAK-Voice-0.1.0-r6-civRelease.apk](./XTAK-Voice-0.1.0-r6-civRelease.apk)

XTAK Voice adds voice-communications capability to XTAK. It is primarily geared toward Token Mesh transport for decentralized and resilient field voice communications, while also supporting—and continuing to expand—compatibility with TAK Voice workflows. Development is ongoing around transport, audio handling, controls, and interoperability.

### XTAK WRAITH

[XTAK-WRAITH-0.2.0-r3-civRelease.apk](./XTAK-WRAITH-0.2.0-r3-civRelease.apk)

XTAK WRAITH is a wireless Remote ID detection and tracking plugin for unmanned aircraft. It scans supported Bluetooth and Wi-Fi Remote ID broadcasts, extracts available aircraft information, and plots detected UAVs in XTAK for local situational awareness.

## Building

XTAK is based on the ATAK CIV 5.5.1.8 Android codebase and uses the Android/Gradle build system.

A typical development environment requires:

- Android SDK
- a compatible JDK
- Gradle dependencies required by the ATAK/XTAK source tree
- appropriate local Android SDK configuration
- signing configuration for release builds

Release signing material is intentionally **not** included in the public source package. Developers building their own APK should configure their own signing credentials locally.

## Installation

Install the release APK on a compatible Android device using your preferred Android deployment method.

For ADB installation:

```powershell
adb install XTAK-5.5.1.8-c1-civ-release.apk
```

For an upgrade over an already installed compatible build:

```powershell
adb install -r XTAK-5.5.1.8-c1-civ-release.apk
```

Android signing compatibility still applies. If an installed build was signed with a different certificate, Android may require that build to be uninstalled before installing another signing lineage.

## Project Status

XTAK is actively developed and may contain experimental or evolving functionality.

Public releases represent specific tested snapshots. Development builds and unreleased features may differ from the public release available here.

## Licensing

XTAK incorporates and modifies software from the ATAK ecosystem and may also include third-party components with their own license requirements.

Users and redistributors are responsible for complying with all applicable licenses included with the source and its dependencies. Refer to the license and notice files contained in the source package for the authoritative terms that apply to individual components.

## Disclaimer

XTAK is an independent project and is not an official TAK Product Center release.

ATAK, TAK, and related names may be trademarks of their respective owners. References to upstream projects are provided for technical identification and compatibility context.

Use this software only in accordance with applicable laws, regulations, licenses, organizational policies, and authorization requirements.
