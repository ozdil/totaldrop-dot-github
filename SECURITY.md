# Security Policy

TotalDrop is an end-to-end encrypted file transfer system. We treat cryptographic, protocol, path-confinement, memory-safety, and supply-chain vulnerabilities with the highest priority.

## Reporting a Vulnerability Privately

**Do NOT open a public GitHub issue for suspected security vulnerabilities.**

Please report vulnerabilities privately through either channel:
1. **GitHub Private Vulnerability Reporting:** [Report a vulnerability](https://github.com/totaldrop-app/totaldrop-core/security/advisories/new) (or the `Security -> Report a vulnerability` tab on the affected `totaldrop-app/*` repository).
2. **Email:** `security@totaldrop.app` (canonical endpoints are also listed in `https://totaldrop.app/.well-known/security.txt`).

Include affected repository/version, reproduction steps or proof-of-concept, and impact assessment. We acknowledge reports within **72 hours** and coordinate disclosure and credit with you once a fix is verified and released.

## Scope & Safe Harbor

- **In Scope:** Cryptographic & PAKE (`CPace`, `Noise XXpsk3`, `ML-KEM-768`, Ghost Ring) flaws, path traversal / symlink escapes, memory unsafety at FFI boundaries, terminal/UI control or Bidi injection, Worker isolation bugs, and reproducible-build / provenance bypasses.
- **Production Safety:** Never perform denial-of-service, fuzzing, or automated volume testing against live `totaldrop.app`, `rendezvous.totaldrop.app`, or `relay.totaldrop.app` endpoints; run reproduction harnesses locally against `totaldrop-servers`.
