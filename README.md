# Candidate Exercise — Pair Programming

**What this session is**

This is a collaborative pair-programming exercise in Python (~45–60 minutes). You'll work through it *with* one of our team members — treat them as a teammate, not an examiner. We're far more interested in how you reason about an open-ended problem and how you work with someone else than in whether you produce perfect or complete code. There's no single right answer, and you are not expected to finish everything.

**What you're working with**

We'll share a notebook/environment with three tables already loaded. They were exported from different systems. There's a short starter notebook that loads the data and shows a quick peek so you can skip setup — everything past that is yours, and you're free to ignore or rework it.

Hagerty writes specialty **insurance** for collector and enthusiast vehicles. Policies run in annual terms and come up for **renewal** each year. The Underwriting team wants to understand which **lead sources** bring in policyholders who go on to renew (rather than lapse), so they can decide where to focus.

`policies`

| column | description |
|---|---|
| `policy_id` | policy identifier |
| `inception_date` | when the policy first took effect |
| `lead_source` | how the policy was originated (e.g. online, direct, agency, broker, club_partner) |
| `program` | underwriting program (standard, modern_classic, collector) |
| `garaging_state` | state where the vehicle is garaged |

`policy_events`

| column | description |
|---|---|
| `policy_id` | policy identifier |
| `event_date` | date of the event |
| `event_type` | `premium_payment`, `renewal`, `claim_paid`, or `premium_refund` |
| `amount` | dollar amount recorded for the event |

A note on `amount`: it's recorded for every event type, but those types don't all mean the same thing — a premium or renewal is money in, a paid claim is a loss paid out, and a refund is money returned. Mind which types you're combining.

`vehicle_risk`

| column | description |
|---|---|
| `policy_id` | policy identifier |
| `vehicle_value` | insured value of the vehicle (USD) |
| `vehicle_era` | e.g. prewar, postwar_classic, muscle, modern_classic, modern |
| `annual_mileage_band` | declared annual mileage band |
| `appraised_value` | appraised value, when an appraisal is on file (USD) |

**The task**

To start: **which lead sources bring in the policyholders most likely to renew?** Get us to a first answer, and we'll take it from there together.

**Tools**

Use whatever you'd normally use, including AI assistants (Copilot, Claude, ChatGPT, etc.) and web search. We use these tools day to day and want to see how you work realistically. The only thing we ask is that you stay able to explain and build on whatever ends up on the screen — your teammate will be curious about the choices being made.

Talking through your thinking as you work makes this much more useful for both of us.
