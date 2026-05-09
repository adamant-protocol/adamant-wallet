# adamant-wallet

The reference wallet for Adamant Protocol.

Self-custody. Default-shielded balances. Sub-second confirmations. Hardware wallet support. Available for desktop (macOS, Windows, Linux) and mobile (iOS, Android).

## Status

Pre-alpha. Under active development.

The wallet is being built as a Tauri-based application with shared core logic in Rust and platform-specific shells for desktop and mobile distribution. No releases yet.

## What this is

A user-facing wallet for sending, receiving, and shielding ADM. Includes view-key management for selective disclosure, transaction history (private to the holder), and integration with the Adamant network for direct chain interaction.

## What this is not

This is not a custodial service. The wallet does not custody your funds — you do. The repository contains the software you run to manage your own keys.

## Architecture

Core wallet logic is implemented as a Rust crate, shared across desktop and mobile builds. Desktop targets use Tauri; mobile targets use a thin native wrapper around the shared core. This allows a single audited codebase to ship across all platforms.

## Build

(Forthcoming.)

## Security

The wallet handles private keys and signs transactions. It is critical security software. Releases will be reproducible builds, signed by the maintainers, and audited prior to mainnet.

Do not use pre-alpha builds with real funds.

## License

Apache License 2.0. See `LICENSE`.

## Links

- Protocol: [adamant](https://github.com/adamant-protocol/adamant)
- Specification: [adamant-spec](https://github.com/adamant-protocol/adamant-spec)
- Project homepage: [adamantprotocol.com](https://adamantprotocol.com)
