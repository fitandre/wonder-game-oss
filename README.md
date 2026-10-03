# wonder-game-oss

Open-source remote desktop, cloud gaming and USB redirection, used from a single web page.

## What it is

- **Desktop mode** — a full Windows desktop in the browser over RDP, using the IronRDP web client behind
  Devolutions Gateway. The user signs in once at the portal; the desktop opens with no second login. Full-duplex
  audio, camera, USB devices, drives and clipboard are enabled by server-side configuration, not by user settings.
- **Game mode** — low-latency game streaming over WebRTC: hardware video encoding (AV1, HEVC, H.264), Opus audio,
  keyboard, mouse and gamepad input that always takes priority over audio and video, and audio/video
  synchronization.
- **USB redirection** — devices plugged into the user's machine reach the remote host (WebUSB in the browser to RDP
  USB redirection).
- **Hosts** — Windows Server 2025 virtual machines on Kubernetes (KubeVirt). Linux and macOS hosts are planned later.
- **Clients** — Chromium-based browsers; the main target is an Android laptop terminal with a hardware AV1 decoder
  running Chromium in kiosk mode.

## Status

Early development. The components are developed in a private repository and are published here as each one is ready
for release. There is nothing to download yet.

## Code signing

Windows binaries released from this repository are planned to be signed through the
[SignPath Foundation](https://signpath.org/) free code signing program for open-source projects. The application has
not been submitted yet; until it is approved, no release from this repository is signed.

## Contributing

The project does not accept outside contributions yet. Issues are welcome.

## License

Apache License 2.0 — see [LICENSE](LICENSE). Third-party components keep their own licences, which will be listed in
this repository as the code arrives.
