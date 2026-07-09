# Orrery 0.1.0-beta Beta

Portable Windows beta build for subscriber testing.

## Assets

- Orrery-0.1.0-beta-win-x64-portable.zip - unzip and run Orrery.exe.
- package-security-report.json - binary-only/obfuscation/leak-audit report.
- release-manifest.json - source/build/entitlement metadata.
- checksums.sha256 - SHA-256 checksums.

## Access Boundary

Orrery requires sign-in. Real agent/model work, hosted Arbiter, DeepSeek, Doubleword credits, managed connectors, cloud runs, and proof-vault features are gated to active trial/subscription plans. Preview mode lets signed-in users inspect setup and product surfaces without consuming cloud capacity.

## Beta Fix In This Build

The packaged sidecar now receives strict entitlement verification config from the bundled public Orrery config, so non-subscribed packaged users remain blocked from real agent/model runs instead of falling back to local routes.

## Hardening Boundary

The public packet is a binary/metadata release: private Orrery source, source maps, TypeScript sources, tests, fixtures, env files, provider keys, API keys, and server secrets are excluded. Paid cloud value is enforced server-side.

## Installer Note

The NSIS installer/update feed is intentionally blocked until a Windows code-signing certificate is configured with CSC_LINK/CSC_KEY_PASSWORD or CSC_NAME. This beta asset is a portable zip built from the packaged app.