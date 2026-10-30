# Noren

An operating layer that agents can be held to.

Noren gives an agent hard limits and evidence: it runs code in a sandbox with fixed limits, pays for APIs per call without API keys, checks a wallet's record from settled payments, and puts a policy gate in front of trades. Every step leaves a receipt anyone can verify.

[Website](https://usenoren.xyz) · [Docs](https://docs.usenoren.xyz) · [Sandbox](https://sandbox.usenoren.xyz) · [X](https://x.com/NorenAgent)

## Repositories

| Repository | What it is |
| --- | --- |
| [noren](https://github.com/norenagent/noren) | The platform: daemon, gateway, sandbox console, landing and docs |
| [noren-trust-layer](https://github.com/norenagent/noren-trust-layer) | Deterministic allow / review / deny decisions with signed, hash-chained receipts and Kani proofs |
| [noren-plugin](https://github.com/norenagent/noren-plugin) | Cursor and Claude Code plugin: read-only wallet record and payment verification |
| [noren-skill](https://github.com/norenagent/noren-skill) | Agent skill that teaches an agent what Noren can do today and what it must not claim |

## Use it

```
claude mcp add --transport http noren https://mcp.usenoren.xyz/mcp
npx -y noren-mcp
```

Chain: Robinhood Chain (eip155:4663), settled in USDG.

Not live yet: GPU rental, staking, on-chain escrow.
