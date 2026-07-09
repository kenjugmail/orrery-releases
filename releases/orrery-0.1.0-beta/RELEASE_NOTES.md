# Orrery 0.1.0-beta Beta

Portable Windows beta build for subscriber testing.

## Assets

- Orrery-0.1.0-beta-win-x64-portable.zip - unzip and run Orrery.exe.
- package-security-report.json - binary-only/obfuscation/leak-audit report.
- release-manifest.json - source/build/entitlement metadata.
- checksums.sha256 - SHA-256 checksums.

## Access Boundary

Orrery requires sign-in. Hosted Arbiter, DeepSeek, Doubleword credits, managed connectors, cloud runs, and proof-vault features are server-gated for active trial/subscription plans. Legacy local access remains local/BYOK only.

## Hardening Boundary

The public packet is a binary/metadata release: private Orrery source, source maps, TypeScript sources, tests, fixtures, env files, provider keys, BYOK keys, and server secrets are excluded. Electron/Node apps remain reverse-engineerable in principle, so paid cloud value is enforced server-side.

## Installer Note

The NSIS installer/update feed is intentionally blocked until a Windows code-signing certificate is configured with CSC_LINK/CSC_KEY_PASSWORD or CSC_NAME. This beta asset is a portable zip built from the obfuscated packaged app.
