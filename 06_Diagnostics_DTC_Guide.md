# Diagnostics & DTC Quick Reference — 2016 F-250 6.2L Gas 4x4

General method: **verify the complaint → scan all modules (not just the PCM) → check TSBs/SSMs/recalls → freeze frame and live data → pinpoint test → repair → verify the repair (drive cycle, monitors complete).**

## Powertrain DTCs most seen on this truck
| DTC | Meaning | 2016 F-250 6.2L specifics / first checks |
|---|---|---|
| P0300–P0308 | Random / cylinder misfire | Plugs (16!), coils (swap test), wet boots, **broken valve spring** (leak-down), injector, vacuum leak; check Mode 6 misfire counts |
| **P0351–P0358**, especially **P0355/P0356** | Ignition coil primary circuit | **TSB 18-2047**: cyl 5/6 connector open from resonator interference |
| P0171/P0174 | System lean, both banks | Vacuum/intake leak after the MAF, dirty MAF, low fuel pressure (FPDM/pump), PCV/valve cover leak, exhaust leak upstream of the O2 sensor |
| P0172/P0175 | Rich | Leaking injector, MAF, high fuel pressure, EVAP purge stuck open |
| P0011–P0024 | Cam timing over-advanced/retarded | Oil level and viscosity (5W-30), VCT solenoid, phaser, timing chain stretch |
| P0016–P0019 | Crank/cam correlation | Timing chain/tensioner/guides, sensor, tone ring |
| P0128 | Coolant below thermostat temperature | Thermostat stuck open, ECT sensor |
| P0420/P0430 | Catalyst efficiency | Exhaust manifold leaks (stud breakage), misfire history, O2 sensors, then catalysts |
| P0455/P0456/P0457 | EVAP leak | Easy Fuel capless filler, CVS vent (mud/insects), purge valve, hoses; smoke test |
| **P0627/P0628/P0629, P025A/P025B, U0109** | Fuel pump control / FPDM | **TSB 16-0060** PCM reprogram (built ≤ 4/6/2016); FPDM corrosion, connector, grounds |
| P2111/P2112/P2135/P2101 | Throttle actuator | Coked throttle body, ETB, connector, APP sensor; **SSM 46085** (don't use ETC PIDs) |
| P264F | ESN not programmed | After PCM replacement (**SSM 47823**) |
| P06A0 | A/C compressor control | **SSM 47850** (EVDC valve test) |

## Transmission DTCs (6R140)
| DTC | Meaning | Notes |
|---|---|---|
| **P0751 / P0730 / P2700** | SSA performance / wrong ratio / apply time | **TSB 16-0057** (built ≤ 12/15/2015) |
| P0711–P0713 | TFT sensor | Internal harness |
| P0715/P0717, P0720/P0722 | Turbine/output speed sensor | Sensor, harness, case connector |
| P0741 | TCC slip | Fluid level/condition, TCC solenoid, converter, reflash |
| P0960–P0977 | Solenoid circuits | Case connector, internal harness, solenoid body |
| P0868 | Line pressure low | Fluid level, pump, filter seal, valve body |
| P0218 | Transmission overtemp | Towing load, cooler restriction, fluid level/condition |

## Chassis / body
| DTC | Meaning | Notes |
|---|---|---|
| C0035/C0040/C0045/C0050 (and C1xxx) | Wheel speed sensor | Rust-jacked tone rings, sensor gap, harness at the knuckle |
| TCCM DTCs (shift motor, encoder, hub solenoid) | 4x4 faults | Shift motor connector corrosion, vacuum hub solenoid circuit |
| B0020 / B1xxx / **B141B/B141C** | SRS circuits | **Clockspring recall 22V337**; TSB160001 (B141B/C) |
| U0100/U0121/U0140, etc. | Lost communication | Battery/grounds, CAN wiring, module power; SSM 45894 (MS-CAN) |

## Symptom-based trees
### Engine cranks, won't start
1. PATS light flashing? (key/BCM: SSM 47824). 2. Fuel pump runs on key-on (2 s prime)? If not, FPDM fuse/relay, FPDM, pump, TSB 16-0060 DTCs. 3. Fuel pressure at the rail (Schrader) vs spec [VERIFY]. 4. Spark (check several coils), CKP signal (RPM PID while cranking). 5. Flooded: hold the accelerator to the floor while cranking (clear-flood). 6. Inertia/crash event (fuel shutoff via RCM; the restart procedure is in the OM).

### Ticking noise
- Cold only, fades when warm, louder under load → **exhaust manifold leak** (broken studs).
- Constant, rpm-related, from the top end → lifter/lash adjuster or rocker roller, **broken valve spring**, injector tick (normal).
- At startup for 1–3 s → VCT phaser/tensioner bleed-down (oil, phaser).

### Oil consumption
- External leaks first (valve covers, rear main, front cover, oil cooler lines). Then PCV: **RH valve cover baffle (2015–2016 builds 3/1/2014–9/8/2015)**, PCV hoses/fittings. Then rings/valve seals (compression/leak-down, spark plug fouling).

### Vibration
- At speed regardless of gear → tires/wheels (balance, runout), **rear driveshaft (also cracks the transmission case/pan, TSB 22-2356)**, U-joints, center bearing.
- In 4x4 only → front driveshaft, front axle U-joints, hubs.
- Shake after bumps at 40–60 mph → **death wobble** tree (`procedures/09_...`).
- At 40–55 mph light throttle, like rumble strips → **torque converter clutch shudder** (P0741 may set).

### Front 4x4 won't engage
- `procedures/08_...` auto-hub flow: LOCK hubs manually → vacuum lines → solenoid → knuckle seals → TCCM/shift motor.

### Brake pedal hard / hissing / no reserve
- Hydro-Boost tree in `procedures/11_...`.

### Overheating while towing
- Fan clutch, radiator/condenser/cooler stack cleanliness, coolant level/air pocket, thermostat, water pump; watch trans temp, since the TorqShift adds heat to the radiator.
