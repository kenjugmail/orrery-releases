# Orrery Releases

Public binary release channel for Orrery desktop.

This repository intentionally does **not** contain Orrery source code. Source,
build scripts, service configuration, provider keys, and release internals stay
in the private/source repositories and Orrery Cloud infrastructure.

## Current Beta

- Release tag: `orrery-0.1.0-beta`
- Artifact: `Orrery-0.1.0-beta-win-x64-portable.zip`
- Platform: Windows x64 portable beta
- Access: sign-in required; active trial/subscription unlocks hosted/cloud
  features. Legacy local access remains local/BYOK only.

## Subscriber Boundary

The download is public for distribution simplicity, but the product value is
server-gated:

- Arbiter hosted credits
- DeepSeek hosted credits
- Doubleword credits
- managed connectors and Away Mode
- cloud runs/research runs
- proof vault and team/admin state

Renderer/local plan claims are not trusted for cloud value.

## Security Posture

Release packets include:

- packaged app only, no source tree
- ASAR packaging plus first-party JS obfuscation
- package leak audit/security report
- SHA-256 checksums
- binary-only release metadata

Installer/update-feed builds are held until Windows code signing is configured.
