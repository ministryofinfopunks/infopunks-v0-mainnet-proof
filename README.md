INFOPUNKS v0 MAINNET PROOF INDEX
Generated: 2026-05-04

Status:
Phase 1: Trust + Proof - CONFIRMED
Phase 2: Coherence + Signal - CONFIRMED
Phase 3: Passport + Routing - CONFIRMED

Network:
Base mainnet / eip155:8453

Asset:
USDC

Facilitator:
CDP

PayTo:
0xe4E8908308a86aB43E5dEb6C0fd0F006786104c3

Canonical live proof surfaces

Specific receipt IDs are generated per paid call and may rotate after redeploy while v0 uses in-memory receipt/event storage. The stable proof targets are the public proof indexes, recent event feeds, receipt lookup templates, discovery manifests, and OpenAPI specs.

Trust Layer:

https://infopunks-x402-adapter-cdp-staging.onrender.com/proof

https://infopunks-x402-adapter-cdp-staging.onrender.com/v1/events/recent

https://infopunks-x402-adapter-cdp-staging.onrender.com/receipts/{receipt_id}

https://infopunks-x402-adapter-cdp-staging.onrender.com/.well-known/infopunks-trust-layer.json

https://infopunks-x402-adapter-cdp-staging.onrender.com/openapi.json

Cognition Layer:

https://infopunks-cognition-layer-x402.onrender.com/proof

https://infopunks-cognition-layer-x402.onrender.com/v1/events/recent

https://infopunks-cognition-layer-x402.onrender.com/receipts/{receipt_id}

https://infopunks-cognition-layer-x402.onrender.com/.well-known/infopunks-cognition-layer.json

https://infopunks-cognition-layer-x402.onrender.com/openapi.json

Passport Layer:

https://infopunks-passport-layer.onrender.com/proof

https://infopunks-passport-layer.onrender.com/v1/events/recent

https://infopunks-passport-layer.onrender.com/receipts/{receipt_id}

https://infopunks-passport-layer.onrender.com/.well-known/infopunks-passport-layer.json

https://infopunks-passport-layer.onrender.com/openapi.json


PHASE 1: TRUST + PROOF
Service:
Infopunks Trust Layer

Live URL:
https://infopunks-x402-adapter-cdp-staging.onrender.com

Endpoint:
POST /v1/resolve-trust

Receipt lookup template:
https://infopunks-x402-adapter-cdp-staging.onrender.com/receipts/{receipt_id}

Proof:
https://infopunks-x402-adapter-cdp-staging.onrender.com/proof

Recent Events:
https://infopunks-x402-adapter-cdp-staging.onrender.com/v1/events/recent

OpenAPI:
https://infopunks-x402-adapter-cdp-staging.onrender.com/openapi.json

Manifest:
https://infopunks-x402-adapter-cdp-staging.onrender.com/.well-known/infopunks-trust-layer.json

Result:
x402 verified through CDP on Base mainnet
Final status: 200
Settlement status: provisional
Bazaar metadata status: included
External Bazaar acceptance: pending_confirmation


PHASE 2: COGNITION LAYER
Service:
Infopunks Cognition Layer

Live URL:
https://infopunks-cognition-layer-x402.onrender.com

Endpoint:
POST /v1/coherence-score

Receipt lookup template:
https://infopunks-cognition-layer-x402.onrender.com/receipts/{receipt_id}

Proof Index:
https://infopunks-cognition-layer-x402.onrender.com/proof

Recent Events:
https://infopunks-cognition-layer-x402.onrender.com/v1/events/recent

Settlement:
settled

Endpoint:
POST /v1/extract-signal

Receipt lookup template:
https://infopunks-cognition-layer-x402.onrender.com/receipts/{receipt_id}

Proof Index:
https://infopunks-cognition-layer-x402.onrender.com/proof

Recent Events:
https://infopunks-cognition-layer-x402.onrender.com/v1/events/recent

Settlement:
settled

Endpoint:
POST /v1/simulate-narrative

Receipt lookup template:
https://infopunks-cognition-layer-x402.onrender.com/receipts/{receipt_id}

Proof Index:
https://infopunks-cognition-layer-x402.onrender.com/proof

Recent Events:
https://infopunks-cognition-layer-x402.onrender.com/v1/events/recent

Settlement:
settled

OpenAPI:
https://infopunks-cognition-layer-x402.onrender.com/openapi.json

Manifest:
https://infopunks-cognition-layer-x402.onrender.com/.well-known/infopunks-cognition-layer.json

Proof Index:
https://infopunks-cognition-layer-x402.onrender.com/proof

Result:
/v1/coherence-score: paid, x402 verified, settled
/v1/extract-signal: paid, x402 verified, settled
/v1/simulate-narrative: paid, x402 verified, settled
All three calls return receipt metadata, result hash, proof URL, settlement reference, and public events.


PHASE 3: PASSPORT + ROUTING
Service:
Infopunks Passport Layer

Live URL:
https://infopunks-passport-layer.onrender.com

Endpoint:
POST /v1/route-agent

Receipt lookup template:
https://infopunks-passport-layer.onrender.com/receipts/{receipt_id}

Proof:
https://infopunks-passport-layer.onrender.com/proof

Recent Events:
https://infopunks-passport-layer.onrender.com/v1/events/recent

OpenAPI:
https://infopunks-passport-layer.onrender.com/openapi.json

Manifest:
https://infopunks-passport-layer.onrender.com/.well-known/infopunks-passport-layer.json

Result:
/v1/route-agent: paid, x402 verified, route decision returned
Decision: route
Selected agent example: agent_b
Discovery metadata includes resource, routeTemplate, pricing, network, asset, and payTo for all paid Passport resources.


SUMMARY
Infopunks v0 has shipped three paid x402 primitives on Base:

1. resolve_trust
2. score_coherence / extract_signal / simulate_narrative
3. route_agent

Together:
Trust Layer       -> who can be trusted?
Cognition Layer   -> what signal matters?
Narrative Layer   -> where is this going?
Passport Layer    -> which agent should act next?

Status:
v0 mainnet proof complete.
