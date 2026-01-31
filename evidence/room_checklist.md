# L4 Room Checklist (Evidence)
Status: Template
Version: 0.1
Scope: Node + immediate room perimeter (L4)
Normative keywords: MUST/SHOULD/MAY (BCP14)

Date (UTC): YYYY-MM-DD
Operator: ___________________
Location (coarse): ___________________   (no exact address)
Node ID: ___________________
Snapshot Ref: perimeter_snapshot.json  (filled by operator)

## A) Required (keep this part strict)

### 1) Physical access
- [ ] Room is dedicated during operation window (no unknown visitors)
- [ ] Node is not left unattended while privileged actions are possible
- [ ] Storage with secrets (keys/backups) is physically separated or locked
- [ ] “Hands-on” tamper surface noted (case, ports, USB headers)

### 2) Radio / proximity surface
- [ ] Wi-Fi disabled at OS level
- [ ] Bluetooth disabled at OS level
- [ ] Wi-Fi/Bluetooth disabled in UEFI/BIOS (or hardware removed/blocked)
- [ ] No proximity pairing/handoffs (phone/watch/headset) in the room
- [ ] Ethernet only (record switch/router model if relevant)

### 3) Power chain (link to diagram)
- [ ] Power chain documented in power_chain_diagram.md
- [ ] Surge protection present
- [ ] Filtering present (or UPS double conversion) where applicable
- [ ] No shared “dirty” loads on same strip (heaters, compressors, etc.)

### 4) Thermal / acoustic leakage hygiene
- [ ] Cooling profile is controlled (no uncontrolled fan ramps)
- [ ] Node placement reduces acoustic broadcast (distance, damping, enclosure)
- [ ] Coil whine / fan resonance noted (qualitative: low/med/high)

### 5) Ports / removable media
- [ ] Unused ports disabled (BIOS/OS) where feasible
- [ ] USB autorun disabled (OS)
- [ ] Removable media policy: NONE / ALLOWLIST / CONTROLLED WINDOW
- [ ] Any temporary device connection is logged as a change record

### 6) Privileges / “cannot” layer
- [ ] Privileged actions require explicit operator step (human-in-the-loop)
- [ ] Rate limits exist for risky actions (network, filesystem, external I/O)
- [ ] Challenge window exists for contested decisions (if applicable)
- [ ] Rollback path exists for any change that alters perimeter

### 7) Evidence integrity
- [ ] Snapshot JSON created/updated (perimeter_snapshot.json)
- [ ] Change JSON created for modifications (perimeter_change.json)
- [ ] Hashes recorded for key configs (where possible)
- [ ] Evidence stored locally (closed-box); shared only as redacted pack

## B) Notes (optional, can be messy)

### “Earth paragraph” (why this is non-optional in practice)
A room perimeter is like a thermal and electrical organism: power quality, heat, airflow, and access define stability.
If the node behaves like an “unbounded heater”, you get oscillations: throttling, brownouts, unexplained faults, and accidental leakage.
This is why L4 is not “policy” — it’s wiring, airflow, time windows, and enforced budgets.

### Bridges (do not delete; these anchor cross-domain reasoning)
- Explicit bridge: Cybernetics (Ashby) → stability requires measurable feedback & limits, not promises.
- Hidden bridge #1: Physiology (Guyton/Hall homeostasis) → fatigue/cooldowns as stabilization primitives.
- Hidden bridge #2: Bayesian discipline (Jaynes) → evidence thresholds before action, not narrative confidence.

Free notes:
- Observed anomalies:
- Constraints in this room:
- Next perimeter improvements:
