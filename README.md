# IW4L for iOS

Experimental native iOS adaptation of [vladtrc/iw4L](https://github.com/vladtrc/iw4L), with touch and controller input and local Wi-Fi multiplayer.

- [Download and setup guide](https://chrisjenkynw.github.io/iw4l-ios/)
- [IPA, modified source and checksums](https://github.com/chrisjenkynw/iw4l-ios/releases/tag/v0.1.0-alpha.1)

**Bring your own Windows MW2 (2009) game data.** No original game data is distributed. The IPA needs to be signed for your device with your own sideloading setup. Large maps require the Increased Memory Limit entitlement to be permitted by the signing profile. Xcode signing was tested; third-party re-signing of this release is not yet verified.

This is an alpha, not a complete or performance-guaranteed port. Rust reached approximately 60 FPS on an iPhone 13 Pro Max; Afghan averaged 43.9 FPS in a two-minute clean-build test and 38 FPS in a longer hot-device test. All maps, extended multiplayer sessions and older devices remain unverified. Campaign and official PC/console/IW4x server compatibility are not included.

The release source archive contains the modified runtime and iOS build project. Configure your own team in Xcode, enable Increased Memory Limit, and use `ios/build.sh`. The source includes native touch/controller controls, LAN discovery and hosting, mobile rendering changes, and memory reductions. Development probes and the unfinished rendering-overlap experiment are excluded.

Original IW4L copyright 2026 vladtrc. Apache-2.0; see [LICENSE](LICENSE), [NOTICE](NOTICE), and [third-party licenses](THIRD-PARTY-LICENSES.txt). Unaffiliated with Activision and the original game developers.
