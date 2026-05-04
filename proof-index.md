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


PHASE 1: TRUST + PROOF
Service:
Infopunks Trust Layer

Live URL:
https://infopunks-x402-adapter-cdp-staging.onrender.com

Endpoint:
POST /v1/resolve-trust

Fresh receipt:
xrc_9c23e3d1-5abc-4d9f-b41e-635be9e0f1bf

Receipt:
https://infopunks-x402-adapter-cdp-staging.onrender.com/receipts/xrc_9c23e3d1-5abc-4d9f-b41e-635be9e0f1bf

Proof:
https://infopunks-x402-adapter-cdp-staging.onrender.com/proof

OpenAPI:
https://infopunks-x402-adapter-cdp-staging.onrender.com/openapi.json

Manifest:
https://infopunks-x402-adapter-cdp-staging.onrender.com/.well-known/infopunks-trust-layer.json

Result:
x402 verified: true
Final status: 200
Settlement status: provisional
Verification level: application_receipt_pending_tx_hash
Bazaar metadata status: included
External Bazaar acceptance: pending_confirmation


PHASE 2: COGNITION LAYER
Service:
Infopunks Cognition Layer

Live URL:
https://infopunks-cognition-layer-x402.onrender.com

Endpoint:
POST /v1/coherence-score

Fresh receipt:
rcpt_263b4835-42ad-46a2-923b-a1369560cd2e

Receipt:
https://infopunks-cognition-layer-x402.onrender.com/receipts/rcpt_263b4835-42ad-46a2-923b-a1369560cd2e

Proof:
https://infopunks-cognition-layer-x402.onrender.com/proof/rcpt_263b4835-42ad-46a2-923b-a1369560cd2e

Settlement:
settled

Endpoint:
POST /v1/extract-signal

Fresh receipt:
rcpt_f9b215d4-b39a-4217-8660-72329493adc8

Receipt:
https://infopunks-cognition-layer-x402.onrender.com/receipts/rcpt_f9b215d4-b39a-4217-8660-72329493adc8

Proof:
https://infopunks-cognition-layer-x402.onrender.com/proof/rcpt_f9b215d4-b39a-4217-8660-72329493adc8

Settlement:
settled

Endpoint:
POST /v1/simulate-narrative

Fresh receipt:
rcpt_8a132191-7cc2-4fda-9f88-0215b5d76885

Receipt:
https://infopunks-cognition-layer-x402.onrender.com/receipts/rcpt_8a132191-7cc2-4fda-9f88-0215b5d76885

Proof:
https://infopunks-cognition-layer-x402.onrender.com/proof/rcpt_8a132191-7cc2-4fda-9f88-0215b5d76885

Settlement:
settled

OpenAPI:
https://infopunks-cognition-layer-x402.onrender.com/openapi.json

Manifest:
https://infopunks-cognition-layer-x402.onrender.com/.well-known/infopunks-cognition-layer.json

Proof Index:
https://infopunks-cognition-layer-x402.onrender.com/proof

Result:
All three Cognition calls returned 200, were x402 verified through CDP on Base mainnet, and include settled receipt references.


PHASE 3: PASSPORT + ROUTING
Service:
Infopunks Passport Layer

Live URL:
https://infopunks-passport-layer.onrender.com

Endpoint:
POST /v1/route-agent

Fresh receipt:
xrc_7ac41db8-b3a4-447c-b871-bb8a60289755

Receipt:
https://infopunks-passport-layer.onrender.com/receipts/xrc_7ac41db8-b3a4-447c-b871-bb8a60289755

Proof:
https://infopunks-passport-layer.onrender.com/proof

OpenAPI:
https://infopunks-passport-layer.onrender.com/openapi.json

Manifest:
https://infopunks-passport-layer.onrender.com/.well-known/infopunks-passport-layer.json

Result:
x402 verified: true
Final status: 200
Decision: route
Selected agent: agent_b
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
