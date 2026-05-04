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
xrc_41855125-159b-4563-82a9-91e05bdfe6cb

Receipt:
https://infopunks-x402-adapter-cdp-staging.onrender.com/receipts/xrc_41855125-159b-4563-82a9-91e05bdfe6cb

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


PHASE 2: COGNITION LAYER
Service:
Infopunks Cognition Layer

Live URL:
https://infopunks-cognition-layer-x402.onrender.com

Endpoint:
POST /v1/coherence-score

Fresh receipt:
rcpt_c964f4f1-f9b5-43a0-ad4a-c81a069edb41

Proof:
https://infopunks-cognition-layer-x402.onrender.com/proof/rcpt_c964f4f1-f9b5-43a0-ad4a-c81a069edb41

Settlement:
settled

Endpoint:
POST /v1/extract-signal

Fresh receipt:
rcpt_347e1ead-1ee0-4c7e-8eae-68025136d428

Proof:
https://infopunks-cognition-layer-x402.onrender.com/proof/rcpt_347e1ead-1ee0-4c7e-8eae-68025136d428

Settlement:
settled

Endpoint:
POST /v1/simulate-narrative

Fresh receipt:
rcpt_532d4af1-c1b4-48f8-84c4-174323f85116

Proof:
https://infopunks-cognition-layer-x402.onrender.com/proof/rcpt_532d4af1-c1b4-48f8-84c4-174323f85116

Settlement:
settled

OpenAPI:
https://infopunks-cognition-layer-x402.onrender.com/openapi.json

Manifest:
https://infopunks-cognition-layer-x402.onrender.com/.well-known/infopunks-cognition-layer.json

Proof Index:
https://infopunks-cognition-layer-x402.onrender.com/proof


PHASE 3: PASSPORT + ROUTING
Service:
Infopunks Passport Layer

Live URL:
https://infopunks-passport-layer.onrender.com

Endpoint:
POST /v1/route-agent

Fresh receipt:
xrc_da0db29e-8f12-4f85-9f09-22da5030c975

Receipt:
https://infopunks-passport-layer.onrender.com/receipts/xrc_da0db29e-8f12-4f85-9f09-22da5030c975

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
