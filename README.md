# Hiroki Kakihara — Financial Infrastructure Engineering

Open-source primitives for high-integrity payment systems, deterministic accounting, and banking protocol interoperability.

## Core Open-Source Suite

- **iso20022-wire-kit** — Zero-dependency TypeScript parser, builder, and strict validator for ISO 20022 messages (pain.001, pacs.008, camt.053).
- **atomic-ledger-engine** — High-throughput Go 1.22 immutable double-entry ledger core with minor-unit arithmetic and Merkle audit proofs.
- **idempotent-pay-guard** — Distributed idempotency-key enforcement middleware compliant with IETF HTTP API specifications.
- **webhook-vault-verifier** — Constant-time signature verification and replay defense for Stripe, Adyen, Wise, and Ed25519 webhooks.
- **recon-stream-core** — Streaming settlement reconciliation engine with multi-currency fee-split tolerance.

## Engineering Guarantees

1. **Zero Floating-Point Money:** Every monetary operation uses integer minor units (`bigint` / `int64`) mapped strictly to ISO 4217 scales.
2. **Zero Runtime Bloat:** Minimalist dependency trees auditable in minutes by bank compliance and security teams.
3. **Deterministic Failure Modes:** Typed error taxonomies and strict schema enforcement against XML external entity (XXE) and replay attacks.

## Sustaining Independent Payment Tooling

If these libraries save your engineering team weeks of compliance and protocol integration work, consider supporting ongoing maintenance via [GitHub Sponsors](https://github.com/sponsors/h-kakihara).
