# Power Chain Diagram (Evidence)
Status: Template
Version: 0.1
Scope: One node + its power path

Date (UTC): YYYY-MM-DD
Operator: ___________________
Node ID: ___________________

## Diagram (fill with real device models)
Grid/Wall
  |
  |-- [Breaker Panel] (ID: ________)
  |
  +-- [Surge Protector] (Model: ________)
        |
        +-- [EMI/RFI Filter] (Model: ________)  (optional)
              |
              +-- [UPS] (Model: ________)  (OFF / Line-interactive / Double-conversion)
                    |
                    +-- [PDU/Strip] (Model: ________)
                          |
                          +-- Node PSU (Model: ________)
                          |
                          +-- (Other loads?)  YES/NO
                                 If YES: list and justify.

## Measurement points (optional but useful)
- Point A (wall): voltage stability notes ______________________
- Point B (post-UPS): noise/transfer notes _____________________
- Point C (node): PSU telemetry / logs _________________________

## Rules (A: strict)
- MUST avoid sharing the strip with noisy loads (heaters, motors, compressors).
- MUST record UPS mode (double-conversion preferred for sensitive ops).
- SHOULD document grounding anomalies if known (hum, coil whine changes).

## Earth paragraph
Power is data. Common-mode noise and brownouts translate into timing drift, throttling, and weird “ghost” failures.
A clean, documented chain makes post-mortems possible and raises the bar for power-line injection classes of attacks.
