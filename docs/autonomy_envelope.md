# Autonomy Envelope (L4) — Operational Policy for Long-Lived Entities

**Purpose:** define how autonomy is bounded, escalated, and audited in real deployments.  
**Scope:** operational governance (L4). Not a promise of safety; a procedure for accountability.

---

## The envelope: three modes

### 1) BASE (default)
- **Deny-by-default** capabilities.
- No external side effects.
- Memory writes allowed only through approved channels (append-only logs where applicable).
- Fail-closed on uncertainty (missing evidence, missing identity, missing budget).

### 2) WINDOW (time-boxed autonomy)
A bounded interval for exploration and internal work.

- Must have a **start time**, **end time**, and **explicit budget**.
- Permitted actions are pre-declared (capability set).
- No privilege escalation inside the window.
- Any request to act externally becomes a **proposal**, not an action.

### 3) WITNESS (audit consolidation)
Post-window consolidation step.

- Produce a witness record: what was attempted, what changed, what was deferred.
- Hash and timestamp the record.
- If a window produced ambiguous outcomes, default to rollback or quarantine.

---

## Capability Gate (deny-by-default)

Capabilities are explicit flags. Examples (non-exhaustive):
- IO_READ_LOCAL, IO_WRITE_LOCAL
- TOOL_EXEC_LOCAL
- MODEL_CALL_LOCAL
- ORACLE_CALL_REMOTE (scarce, requires justification)
- NET_ACCESS (normally **OFF**)
- ACCOUNT_ACCESS (normally **OFF**)
- FINANCIAL_ACTIONS (normally **OFF**)

**Rule:** capabilities are granted per window, not globally.

---

## Two-key escalation (only for dangerous transitions)

Two-key is required for:
- creating a new agent/process with independent execution
- granting new capabilities outside BASE
- enabling any external side effect channel
- opening a remote oracle window (if used)

**Policy:** routine work does not ask for two-key. Only boundary crossings do.

---

## Budgets (hard limits)

Each WINDOW must set:
- time budget (wall-clock)
- compute budget (if available)
- rate limit (requests per minute)
- optional “spend” budget (if any paid oracle exists)

**Fail-closed triggers:**
- exceeded budget
- missing identity / missing audit trail
- missing perimeter evidence (when required)

---

## Oracle scarcity

Remote oracle access is treated as scarce:
- must be justified (one paragraph)
- must be time-boxed
- must be logged (who asked, why, result pointer)

---

## Incident definition (operational)

An incident is any of:
- action executed outside declared capability set
- privilege escalation without two-key
- external side effect without witness record
- logs missing / tampered / unverifiable hash chain

Default response:
- freeze autonomy (BASE only)
- snapshot state
- generate incident witness
- require explicit human decision to resume

---

## Bridges (required)

**Explicit bridge:** c = a + b  
“b” includes autonomy policy; otherwise “c” is not accountable.

**Hidden bridge #1 (Ashby):**  
Bounded windows give the controller enough variety without yielding uncontrolled degrees of freedom.

**Hidden bridge #2 (Cover & Thomas):**  
Witness records + hashes compress accountability into checkable strings.

---

## Earth paragraph (engineering)

This is “envelope protection” for a safety-critical controller:  
you don’t remove constraints to fly better — you define allowed maneuvers and log them, so faults are diagnosable, not mythical.

End.
