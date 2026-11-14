# Governance

TotalDrop is an independent open-source project governed openly on GitHub in **English** ([ADR 0019](https://github.com/totaldrop-app/totaldrop-core/blob/main/docs/decisions/0019-english-by-default.md)).

## Roles

- **Contributors:** Anyone who reports issues, reviews translations across our 35 supported languages, submits pull requests, or audits security models and packaging recipes.
- **Sub-Platform & Area Maintainers:** Engineers responsible for specific client platforms (`Linux`, `Android`, `Windows`, `macOS`, `iOS/tvOS`, `CLI/BSD`, `Web WASM`), sub-platform × CPU packaging (`x86_64`, `arm64`, `riscv64`), localization (`l10n`), or formal verification (`Tamarin` / `cargo-fuzz`).
- **Core Maintainers (`@totaldrop-app/maintainers`):** Steward cryptographic and protocol integrity, approve Architecture Decision Records (`docs/decisions/`), and guard production release environments (`cloudflare`, `linux-release`, `play-release`, `windows-release`, `apple-release`).

## Decision-Making

1. **Technical Consensus & ADRs:** Changes to protocol wire formats, cryptographic primitives, threat-model assumptions, or cross-repository architecture require an English Architecture Decision Record in [`totaldrop-core/docs/decisions/`](https://github.com/totaldrop-app/totaldrop-core/tree/main/docs/decisions).
2. **Independent Review Rule:** No pull request touching code, CI workflows, packaging recipes, or security policy merges without an independent review from a maintainer or review session that did not write the change.
3. **Financial Independence (`ADR 0005`):** TotalDrop accepts no venture capital, ads, or paid feature tiers. Donations never grant governance authority or roadmap priority.
