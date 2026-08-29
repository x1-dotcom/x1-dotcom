# X1 // EVIDENCE AND TRUST

X1 separates engineering state, runtime proof and commercial availability deliberately.

> **EVIDENCE > ASSUMPTION**

A source file, a passing test, a successful deployment and an available commercial capability are not interchangeable facts.

## Evidence states

| State | What it means | What it does not prove |
|---|---|---|
| `IMPLEMENTED` | The capability exists in source or a product implementation. | That the exact production runtime is running it. |
| `TESTED` | An appropriate test exercised defined behaviour. | That every real production target/customer flow behaves identically. |
| `RUNTIME VERIFIED` | The relevant behaviour was observed on the intended runtime/target. | That the capability is automatically commercially available everywhere. |
| `PRODUCTION AVAILABLE` | The capability is approved for current customer-facing use. | Unlimited scope, universal compatibility or unrelated entitlements. |
| `FOUNDATION / PRIVATE PREVIEW / ROADMAP / UNKNOWN` | A deliberately weaker or unresolved state. | Current production availability. |

The core rule is:

```text
IMPLEMENTED != TESTED != RUNTIME VERIFIED != PRODUCTION AVAILABLE
```

## Practical examples

### Device control

```text
COMMAND ACCEPTED != DEVICE ACTION VERIFIED
```

A control plane accepting a command proves that the command entered the control path. It does not by itself prove that the target device executed the requested action successfully.

### Commercial price

```text
DOCUMENTED PRICE != CURRENT CHECKOUT FACT
```

Documentation can record an approved commercial value at a point in time. When the question is what checkout charges now, the current Store/commerce authority must answer it.

### Future capability

```text
SPECIFICATION EXISTS != CAPABILITY AVAILABLE
```

A detailed design or Git branch can be useful engineering evidence without being a current customer-facing availability claim.

---

## Signed licence snapshots — a bounded production proof

One X1 licensing foundation has stronger evidence than source/test alone: the **generic signed licence/snapshot transport chain** has been exercised end to end against production infrastructure.

The recorded production exercise included:

- SaaS licence identity reaching the provisioning path;
- a signed snapshot being fetched by the target panel;
- signature verification;
- persistence of the verified snapshot by the target runtime.

Safe claim:

> **The generic signed licence/snapshot transport foundation has E2E production evidence.**

This is useful because signed commercial/entitlement state can travel through the intended verification path without asking the target runtime to trust an unsigned, manually copied or model-generated feature list.

### What that proof does not mean

It does **not** prove that every paid plugin has a production-verified purchase/suspend/unsuspend/terminate lifecycle or that snapshot transport alone proves each plugin's runtime effect.

Different layers can have different evidence levels at the same time:

| Layer | Current bounded statement |
|---|---|
| Generic signed snapshot transport | E2E production evidence exists. |
| Generalized plugin lifecycle bridge | Source + test evidence exists in the recorded evidence set. |
| Exact bridge deployment/lifecycle parity | Requires its own deployment and controlled lifecycle proof. |
| Target plugin runtime effect | Requires per-plugin target evidence. |

The stronger closure path for a plugin lifecycle is:

```text
RUNNING BUILD IDENTITY
-> LIVE PRODUCT/PID MAPPING
-> CONTROLLED LIFECYCLE
-> SIGNED SNAPSHOT TRANSITIONS
-> TARGET RUNTIME GATE
-> AUDIT TRAIL
```

The point is not to weaken real evidence. The point is to prevent one proven foundation from being expanded into a stronger universal claim it does not support.

---

## X1 trust rule

Claims should stop at the strongest state actually proven.

That means:

- source stays source until tested;
- tests stay tests until the intended runtime is observed;
- runtime proof stays scoped to the exact target/surface exercised;
- commercial availability requires the relevant commercial authority;
- limitations stay attached to the proof that needs them.

**Proof is strongest when the limitation travels with it.**

---

X1 // SOFTWARE · SYSTEMS · OPERATIONS
