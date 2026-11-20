# 2016 Ford F-250 Super Duty Lariat 4x4 — 6.2L Gasoline — Repair Knowledge Base

Built 2026-11-20 as the corpus for an AI repair agent. Total size is well under the 2.5 GB budget (see `99_Sources_Gaps_and_Expansion.md` for what to add with the remaining space).

## Truck covered
- 2016 F-250 Super Duty (P2 platform, 2011–2016 generation; **steel body**, not the 2017+ aluminum truck)
- Lariat trim, 4x4, **6.2L 2-valve SOHC gasoline V8** (VIN engine code **6**, flex-fuel capable)
- **6R140 TorqShift 6-speed automatic** (transmission code **P** on the door-jamb label)
- Electronic shift-on-the-fly (ESOF) transfer case, auto/manual vacuum locking front hubs
- Dana 60-type solid front axle (coil springs, radius arms, track bar); Ford/Sterling 10.50" rear axle

## Confidence tags used throughout
| Tag | Meaning |
|---|---|
| **[OM]** | Verified from Ford's official 2016 Super Duty Owner's Manual (2nd printing, Aug 2015), included in `sources/ford_official/` |
| **[TSB]** | From a Ford bulletin/SSM/recall filed with NHTSA (`sources/nhtsa/`) |
| **[FIELD]** | Consensus from technicians, rebuilders, and owner forums. Usually right, but not factory-verified |
| **[VERIFY]** | Plausible or commonly quoted value that conflicts between sources or isn't confirmed for 2016. The agent must tell the user to confirm it in the Ford Workshop Manual (WSM) before relying on it (especially torque on safety parts) |

## File map
| File | Contents |
|---|---|
| `AGENT_SYSTEM_PROMPT.md` | System prompt / operating rules for the repair agent |
| `01_Vehicle_Profile.md` | Configuration, VIN decode, component IDs, how to confirm options |
| `02_Specifications_Fluids_Parts_Torque.md` | Capacities, fluids, Motorcraft parts, engine specs, torque tables |
| `03_Maintenance_Schedule.md` | Ford normal and severe schedules for the 6.2L, plus practical additions |
| `04_TSBs_SSMs_full_list.md` | **All** Ford bulletins on file with NHTSA for 2016 F-Super Duty, grouped by system, with applicability flags (generated) |
| `04a_Recalls.md` | Safety recalls for the 2016 F-250 SD |
| `05_Key_TSBs_and_Known_Problems.md` | Curated list of the bulletins and failure patterns that matter for this truck |
| `06_Diagnostics_DTC_Guide.md` | DTC quick reference and symptom→cause diagnostic trees |
| `procedures/` | System-by-system repair, replacement and rebuild procedures |
| `08_NHTSA_Complaint_Patterns.md` | 291 owner complaints to NHTSA, grouped by component (generated) |
| `99_Sources_Gaps_and_Expansion.md` | Sources, what's missing (the factory WSM and wiring), and how to add it legally |
| `sources/ford_official/` | Owner's Manual PDF plus text extractions, Quick Reference Guide |
| `sources/nhtsa/` | Raw JSON: filtered TSB index, complaints, recalls |

## Loading into an agent
- **Simple:** put every `.md` file into a Claude Project or knowledge base, and use `AGENT_SYSTEM_PROMPT.md` as the instructions.
- **RAG:** chunk the `.md` files on `##`/`###` headings (they're written to be self-contained per heading). Index `sources/ford_official/*_readingorder.txt` in ~1,500-character chunks. The JSON files are good for structured lookup (bulletin number → summary).
