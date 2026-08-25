# Experience Bidding

## Give the bidder a memory

**Status:** `ADVANCE / TEST`  
**Type:** buyer-side product hypothesis on existing market rails

### Possibility

Advertising systems make huge numbers of decisions, but an individual bid opportunity does not necessarily arrive with a clean economic memory of what previous advertising already accomplished toward the advertiser’s goal.

That can cause the system to repeatedly value the next impression as if prior actions did not change what the next action is worth.

### Mechanism

Keep the external market unchanged.

A normal bid request arrives. The bidder resolves advertiser-scoped longitudinal state from information already available to it, combines prior history, provisional progress, pending actions, and observed outcomes with the campaign’s existing objective, and asks:

> **What can this next eligible action still add?**

The bidder then returns an ordinary bid, adjusted bid, eligible choice, or no-bid.

No new publisher field. No new exchange protocol. No advertiser journey object. No new universal identity requirement.

### Proof

Run persistent Control / Treatment experiments using the same campaign configuration.

**Control:** ordinary campaign decisioning.  
**Treatment:** ordinary campaign decisioning plus longitudinal economic state.

Primary success condition:

> The campaign-configured goal improves versus Control while delivery, budget, privacy, policy, latency, and reliability constraints remain within guardrails.

The configured goal may be revenue, conversion, reach, attention, completed view, lift, or another existing advertiser objective.

### Kill test

Narrow or reject the product if:

- longitudinal state does not create material incremental value versus Control;
- latency, identity continuity, state quality, or operational complexity erases the gain;
- existing bidder functions already produce equivalent results; or
- the same benefit can be achieved more simply without a distinct state layer.

### Why it matters

Experience Bidding is intentionally conservative architecturally.

Before arguing that advertising needs new market rails, prove that giving the existing bidder better memory creates value on the rails that already exist.

That makes it both a product hypothesis and a bridge experiment for larger questions about the future transaction architecture.

### Public boundary

This is a research product hypothesis, not a claim of deployment, adoption, patentability, or performance by any specific DSP or advertiser.
