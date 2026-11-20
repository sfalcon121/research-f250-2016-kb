# Scan Tools, Module Programming and Relearns

## Tools
| Tool | Use |
|---|---|
| **Ford IDS** (with VCM II/VCM 3) | Official dealer tool for 2016 SD (FDRS also supports many 2016 modules [VERIFY]). Needs a **Motorcraftservice.com PTS + IDS software license** (short-term licenses available). Required for PMI, PCM reflash per TSB, PATS, ABS bleed, BCM reprogram. |
| **FORScan** (PC + ELM327/J2534 adapter with an MS-CAN switch) | Ford-specific DIY tool: reads all modules, service functions (ABS bleed, KAM reset, misfire monitor relearn, DPF n/a, injector codes n/a for gas), As-Built configuration edits, PATS with an extended license. Many TSB reflashes still need IDS/FDRS calibration files. |
| Generic OBD-II | P-codes, freeze frame, Mode 6 misfire counts. Can't see B/C/U codes in all modules. |
| J2534 pass-thru | Ford calibration downloads via Motorcraftservice (subscription) |

## Procedures that need a scan tool
| Job | Procedure |
|---|---|
| PCM replacement | **PMI** (Programmable Module Installation): original module in, start session, run PMI, install new module when prompted (**SSM 51947**). Program **ESN** (P264F, **SSM 47823**). PATS parameter reset. Misfire monitor relearn. |
| BCM replacement | PMI, PATS parameter reset (all keys present), TPMS sensor training, As-Built check |
| TSB reflashes | 16-0060 (PCM, P0627/U0109), 16-0057 (TorqShift DTCs), SSM 46236 (BCM plow/winch), SB-45316 (APIM/radio) |
| Transmission | Adaptive table reset after repairs, solenoid body/valve body ID or strategy update [VERIFY], fluid temp PID for level check |
| ABS | Service bleed after HCU replacement or air in the unit; steering angle sensor calibration |
| Engine | KAM reset, misfire monitor (CKP) relearn, idle relearn after throttle body work, VCT tests |
| TPMS | Sensor training (OM procedure or TPMS tool). 2016 SD sensors are 315 MHz [VERIFY]. |
| 4x4 | TCCM self-test, shift motor/encoder diagnostics |
| Body | Key programming, door/mirror module config, As-Built for options (e.g. adding tow mirror functions) |
| Battery | BMS reset after replacement (if equipped [VERIFY]) |

## Getting factory calibrations/TSBs legally
- **motorcraftservice.com**: subscriptions (short-term to annual) give the **Workshop Manual, wiring diagrams, PC/ED manual, full TSB/SSM text, and IDS/FDRS software and calibrations**.
- A Ford dealer can run **OASIS by VIN** for open recalls, CSPs, warranty extensions, and applicable TSBs/SSMs.
