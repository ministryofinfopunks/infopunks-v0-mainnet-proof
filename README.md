# Infopunks v0 Mainnet Proof

Canonical public proof directory for the Infopunks v0 x402-paid machine-callable stack on Base.

## Live System

```text
Network: Base mainnet
Network CAIP-2: eip155:8453
Asset: USDC
Facilitator: CDP x402
PayTo: 0xe4E8908308a86aB43E5dEb6C0fd0F006786104c3
Confirmed Phases
Phase 1: Trust + Proof        CONFIRMED
Phase 2: Coherence + Signal   CONFIRMED
Phase 3: Passport + Routing   CONFIRMED
```

## Canonical Live Proof Surfaces

Specific receipt IDs are generated per paid call and may rotate after redeploy while v0 uses in-memory receipt/event storage.

The stable proof targets are:

- public proof indexes
- recent event feeds
- receipt lookup templates
- discovery manifests
- OpenAPI specs

Trust Layer:

```text
https://infopunks-x402-adapter-cdp-staging.onrender.com/proof
https://infopunks-x402-adapter-cdp-staging.onrender.com/v1/events/recent
https://infopunks-x402-adapter-cdp-staging.onrender.com/receipts/{receipt_id}
https://infopunks-x402-adapter-cdp-staging.onrender.com/.well-known/infopunks-trust-layer.json
https://infopunks-x402-adapter-cdp-staging.onrender.com/openapi.json
```

Cognition Layer:

```text
https://infopunks-cognition-layer-x402.onrender.com/proof
https://infopunks-cognition-layer-x402.onrender.com/v1/events/recent
https://infopunks-cognition-layer-x402.onrender.com/receipts/{receipt_id}
https://infopunks-cognition-layer-x402.onrender.com/.well-known/infopunks-cognition-layer.json
https://infopunks-cognition-layer-x402.onrender.com/openapi.json
```

Passport Layer:

```text
https://infopunks-passport-layer.onrender.com/proof
https://infopunks-passport-layer.onrender.com/v1/events/recent
https://infopunks-passport-layer.onrender.com/receipts/{receipt_id}
https://infopunks-passport-layer.onrender.com/.well-known/infopunks-passport-layer.json
https://infopunks-passport-layer.onrender.com/openapi.json
```

## Phase 1: Trust Layer

Service:

```text
https://infopunks-x402-adapter-cdp-staging.onrender.com
```

Paid resource:

```text
POST /v1/resolve-trust
```

Live proof:

```text
https://infopunks-x402-adapter-cdp-staging.onrender.com/proof
```

Recent events:

```text
https://infopunks-x402-adapter-cdp-staging.onrender.com/v1/events/recent
```

Receipt lookup template:

```text
https://infopunks-x402-adapter-cdp-staging.onrender.com/receipts/{receipt_id}
```

Discovery manifest:

```text
https://infopunks-x402-adapter-cdp-staging.onrender.com/.well-known/infopunks-trust-layer.json
```

OpenAPI:

```text
https://infopunks-x402-adapter-cdp-staging.onrender.com/openapi.json
```

Status:

- x402 verified through CDP on Base mainnet
- Final status: 200
- Settlement status: provisional
- Bazaar metadata status: included
- External Bazaar acceptance: pending_confirmation

## Phase 2: Cognition Layer

Service:

```text
https://infopunks-cognition-layer-x402.onrender.com
```

Paid resources:

```text
POST /v1/coherence-score
POST /v1/extract-signal
POST /v1/simulate-narrative
```

Live proof:

```text
https://infopunks-cognition-layer-x402.onrender.com/proof
```

Recent events:

```text
https://infopunks-cognition-layer-x402.onrender.com/v1/events/recent
```

Receipt lookup template:

```text
https://infopunks-cognition-layer-x402.onrender.com/receipts/{receipt_id}
```

Discovery manifest:

```text
https://infopunks-cognition-layer-x402.onrender.com/.well-known/infopunks-cognition-layer.json
```

OpenAPI:

```text
https://infopunks-cognition-layer-x402.onrender.com/openapi.json
```

Status:

- /v1/coherence-score: paid, x402 verified, settled
- /v1/extract-signal: paid, x402 verified, settled
- /v1/simulate-narrative: paid, x402 verified, settled

All three Cognition calls return receipt metadata, result hash, proof URL, settlement reference, and public events.

## Phase 3: Passport Layer

Service:

```text
https://infopunks-passport-layer.onrender.com
```

Paid resources:

```text
POST /v1/passport/register
POST /v1/passport/attest
POST /v1/verify-claim
POST /v1/route-agent
```

Live proof:

```text
https://infopunks-passport-layer.onrender.com/proof
```

Recent events:

```text
https://infopunks-passport-layer.onrender.com/v1/events/recent
```

Receipt lookup template:

```text
https://infopunks-passport-layer.onrender.com/receipts/{receipt_id}
```

Discovery manifest:

```text
https://infopunks-passport-layer.onrender.com/.well-known/infopunks-passport-layer.json
```

OpenAPI:

```text
https://infopunks-passport-layer.onrender.com/openapi.json
```

Status:

- /v1/route-agent: paid, x402 verified, route decision returned
- Decision: route
- Selected agent example: agent_b
- Discovery metadata includes resource, routeTemplate, pricing, network, asset, and payTo for all paid Passport resources.

## Proof Model

This repo does not pin concrete receipt IDs because v0 receipt/event storage may reset after redeploy.

Instead, it points to stable machine-readable proof surfaces:

```text
/proof
/v1/events/recent
/receipts/{receipt_id}
/.well-known/...
/openapi.json
```

## Status

Infopunks v0 mainnet proof is confirmed across three paid machine-callable layers:

- Trust Layer: resolves trust before agents act
- Cognition Layer: turns narrative and market noise into machine-usable signal
- Passport Layer: verifies identity/claims and routes agents

All phases are exposed as public x402-paid resources on Base using USDC and CDP x402.
