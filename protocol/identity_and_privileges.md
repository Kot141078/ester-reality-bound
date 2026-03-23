# Identity and privileges

Real failures happen through channels:
- identity leakage
- privilege drift
- workflow shortcuts
- network surfaces
- supply chains

Therefore:
- identity must be verifiable (not only “user says so”)
- privileges must be explicit and auditable
- escalation must be deliberate, logged, rate-limited

## Operational clarification
- privileges should not be granted to an unbounded swarm as if the swarm were the subject
- in a `c = a + b` system, `c` holds and delegates bounded privileges to agents
- delegation must be scoped, logged, reviewable, and revocable
