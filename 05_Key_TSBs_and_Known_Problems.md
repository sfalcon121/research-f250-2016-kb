# Key TSBs, SSMs, Recalls and Known Problems — 2016 F-250 6.2L Gas 4x4

Curated from `04_TSBs_SSMs_full_list.md` (NHTSA filings) plus field experience. Always confirm VIN and build-date applicability with a dealer (OASIS).

## A. Safety recalls (free at Ford dealers) [TSB]
| NHTSA # | Ford # | Issue | Remedy |
|---|---|---|---|
| **22V337** | 22S35 | Dust in the steering wheel **clockspring** can disconnect the driver airbag circuit; airbag may not deploy. Typical signs: airbag warning light with a driver-airbag circuit DTC, horn or steering-wheel switches intermittent. | Replace clockspring |
| **25V572** | 25S89 | **Rear-view camera** image may fail to display (expands 25V270) | Inspect/replace camera |
| 16V246 | 16S17 | Tires on trucks built Apr 5–11, 2016 may have sidewall damage | Inspect/replace tires |
| 20E090 | (Icon) | Aftermarket Icon 2.5 stabilizer kit 65050 | Only if that kit is installed |

## B. Engine / emissions (6.2L)
| Bulletin | Symptom / DTC | Cause | Fix |
|---|---|---|---|
| **TSB 18-2047** (2014–2016 F-250/350 6.2L) | MIL, **P0355 and/or P0356** (coil E/F primary) | Open circuit in the **coil-on-plug connectors for cylinders 5/6** from rubbing on the **intake air expansion resonator** | Repair/replace connectors and pigtails per TSB; reroute/clear the resonator |
| **TSB 16-0060** (2012–2016 SD 6.2L/6.8L built ≤ 4/6/2016) | MIL with **P0627, P025A, P025B, U0109** | Fuel pump control / FPDM communication calibration | **Reprogram PCM** (and FPDM if called for) to the latest calibration |
| **SSM 46085** | ETB diagnosis | Don't use ETC_ACT/ETC_DSD PIDs to condemn a throttle body; the PCM monitors more accurately | Diagnose by DTCs only |
| **SSM 46295** | Oil leak diagnosis | New white fluorescent engine oil dye available | Use dye to separate oil leaks from other fluids |
| **SSM 47823** | **P264F** after PCM replacement | Engine serial number not programmed | Program ESN into PCM |
| **SSM 51947** | PCM PMI "Configuration Failed" | Wrong module replacement order | Original PCM installed → new session → run PMI |
| Reported TSB (**15-0161**, number not confirmed in NHTSA data) | **Excessive oil consumption**, 2015–2016 SD 6.2L built 3/1/2014–9/8/2015 | **Internally leaking baffle in the RH valve cover**, which pulls oil through the PCV | Replace RH valve cover [FIELD]. Mixed owner results; also check PCV hoses/fittings. |
| [FIELD] | Misfire on one cylinder, ticking, low compression on one cylinder | **Broken valve spring** (known on 2011–2012 builds, occasional later) | Leak-down/compression test; replace spring on-engine with air in cylinder; inspect rocker/valve |
| [FIELD] | Random/single misfire P0300–P0308, worse when wet | Moisture or corrosion in coil boots, worn plugs, coil failure | Swap coil to confirm, replace plugs as a set, dielectric grease on boots |
| [FIELD] | Cold-start exhaust tick that fades when warm | **Broken exhaust manifold studs/bolts or cracked manifold** (LH more common) | Replace manifold and studs. Drill/extract broken studs; heat and penetrant; new gaskets. |
| [FIELD] | Seized/broken spark plugs | Long intervals in aluminum heads | Remove warm-not-hot, use penetrant, slow quarter turns; thread repair inserts if stripped |

## C. Transmission (6R140) and driveline
| Bulletin | Symptom / DTC | Cause / Fix |
|---|---|---|
| **TSB 16-0057** (also filed as TSB160057; 2009–2016 E-Series/F-SD TorqShift built ≤ 12/15/2015) | MIL with **P0751, P0730 and/or P2700** | Shift solenoid A / incorrect gear ratio / friction element apply time. Follow TSB: typically **PCM reprogram** and, if DTCs persist, valve body/solenoid repair [VERIFY specific steps in the full TSB] |
| **SB-45259** (2015 SD TorqShift 6) | High-pitch noise | Per bulletin (applies to 2015; read the full text to see if 2016 builds are included) |
| **SSM 46451** (2009–2017 6R80/6R100/6R140) | Shift complaints | **Updated main control valve body overhaul procedure** (WSM 307-01). Not all valve bodies need replacing; inspect bores, springs, and valves (GSB G0000093 video) |
| **SSM 47976** | Flexplate cracking after transmission R&R | **Grease the converter pilot hub with XL-5-A** and verify dowel pins on every transmission install |
| **TSB 22-2356** (2015–2019 SD) | **ATF leak from a cracked transmission case or pan** | Root cause is **rear driveshaft imbalance**; replace the rear driveline per TSB along with the case/pan |
| **SSM 53040** (2012–2024) | Seal kit on transmission repair | Note on seal kit usage (see full list) |
| [FIELD] 6R140 failure points | Coast clutch, intermediate shaft/input shaft wear, torque converter, high-pressure pump, valve body bore wear (ZF-like) | See `procedures/07_Transmission_6R140.md` |

## D. 4x4, hubs, axles, suspension, steering
| Bulletin | Issue | Fix |
|---|---|---|
| **SSM 46345 / 47979 / 48494 / 49495** (2005–2021 SD 4x4) | **Accelerated vacuum hub seal and wheel bearing wear** in dust, mud, or sand | **Knuckle seal shield kit GC3Z-54024A38-A** (customer-pay) |
| [FIELD] | Auto hubs won't lock (4x4 light on, front not driving) | Cracked/brittle vacuum lines at the knuckle, hub vacuum solenoid, failed spindle/vacuum seals, connector. Spec: hub circuit should hold ≥10 inHg [FIELD]. Workaround: turn hubs to LOCK. |
| **15-0117** (2011–2016 F-250) | Rear sits low under light load | Bulletin information on spring height. Check the full TSB; usually "normal design" plus spring options |
| **PC-01.12.2016** (aftermarket supplier communication for **lifted** 2005–2016 SD 4WD) | Steering wheel oscillation ("**death wobble**") | Track bar, damper, caster correction for lifted trucks. See `procedures/09_Steering_Suspension_Death_Wobble.md` |
| [FIELD] death wobble (stock height) | Violent shake after bumps at 40–60 mph | Track bar ball joint/bushing wear, loose track bar bolts, worn ball joints, tie-rod/drag-link ends, steering box mount, tire balance/runout, low caster, weak damper (damper masks it; it isn't the root fix). Ford's 2017+ TSB 18-2268 (damper) does not cover 2016. |
| **SSM 45900** (2011–2016 SD with running boards) | Rocker/sill damage off-road | Body repair guidance |
| **SSM 52188** | Power steering fluid note: 2024 SD use XL-22. **Not this truck**; 2016 uses MERCON LV [OM]. | — |

## E. Electrical / body / comfort
| Bulletin | Issue | Fix |
|---|---|---|
| **SSM 47886** (2012–2016 SD), **SSM 48123** | **Positive battery clamp corrosion** | Replace only the clamp (BT4Z-14450-AA, negative BT4Z-14450-BA); crimp and heat-shrink. Don't shorten the cable. |
| **SSM 45894** (2016 SD built ≤ 5/1/2016) | Inoperative blower motor, power-fold mirror, RKE fob, or no MS-CAN communication | Per SSM (wiring/module). Check the MS-CAN network |
| **SSM 46236** (2015–2016 SD built ≥ 8/22/2014 with plow/winch) | Panel lights flicker when the accessory runs | **Reprogram BCM** (IDS 103.02+) |
| **SSM 47824** (2015–2017) | No-crank; key programming fails with "Error 232: Key Table Not Allocated" | **BCM internal fault, replace BCM** |
| **SB-45316 / ASI-45241** (2016 SD) | SiriusXM/radio inoperative | Update as-built data / APIM via IDS |
| **SSM 46092** (2016 SD) | SYNC Bluetooth/voice issues | Per SSM (APIM software) |
| **16B10** (CSP) | FCDIM programmed for Europe | Reprogram module |
| **TSB160001** (Mar 2016 monthly comms) | Airbag light with **B141B/B141C** | Per bulletin (RCM/seat-belt pretensioner circuit) [VERIFY] |
| **SSM 47850** | Poor A/C, **P06A0** | EVDC compressor control valve; test with Rotunda 339-EVDC100 before replacing the compressor [VERIFY that the 6.2L uses EVDC] |
| **SSM 51536** | — | Swapping modules between vehicles for diagnosis can lock them (2000–2024) |

## F. Top complaint categories from owners (NHTSA, 291 complaints, all 2016 F-250 SD)
Steering (118 rows; mostly death wobble), suspension (110), unknown/other, air bags (clockspring), engine, electrical, fuel/propulsion (several are 6.7L high-pressure fuel pump, which doesn't apply), wheels, power train, wipers, back-over camera. See `08_NHTSA_Complaint_Patterns.md`.
