# Brakes — 4-Wheel Disc, Hydro-Boost, ABS/AdvanceTrac (2016 F-250)

WSM: 206-00 general, 206-03 front disc, 206-04 rear disc, 206-05 parking brake, 206-07 power brake actuation (Hydro-Boost), 206-09 ABS. Brake fluid **DOT 3 PM-1-C or (recommended) DOT 4 LV PM-20** [OM].

## System
- Front: twin-piston sliding calipers on anchor brackets; vented rotors (hat style over the unit hub [VERIFY]).
- Rear: calipers on anchor plates; rotor with **drum-in-hat parking brake** shoes.
- **Hydro-Boost:** booster powered by power steering pump pressure (MERCON LV), with an **accumulator** that gives 2–3 assisted stops with the engine off. Booster lines connect the pump → booster → steering gear.
- ABS hydraulic control unit + module (ABS/AdvanceTrac with Roll Stability Control). Wheel speed sensors at each hub.

## Pad and rotor replacement (front)
1. Loosen lugs, lift, support, wheel off. Open the bleeder or push fluid back carefully (watch the reservoir level; ideally open the bleeder and clamp the hose to avoid pushing contaminated fluid into the ABS unit).
2. Remove the caliper guide pin bolts, hang the caliper. Remove the pads and the anchor bracket (bolts are **high-torque, often single-use** per WSM [VERIFY]).
3. Remove the rotor. Clean the **hub face of all rust** (runout causes pulsation). Measure rotor thickness against the **minimum stamped on the rotor**; machine or replace.
4. Clean and lubricate the anchor-bracket abutments (high-temp brake grease) and the guide pins (silicone brake lube, not petroleum). New hardware clips.
5. Install the bracket (~166 lb-ft new bolts [FIELD; VERIFY]) and caliper bolts (~55 lb-ft [FIELD; VERIFY]). Lugs 165 lb-ft [OM] in a star pattern.
6. Pump the pedal before moving. **Bed in** the pads (e.g., 8–10 stops from 40 to 10 mph without stopping fully, then cool-down drive).

## Rear pads/rotors and parking brake
- Same approach; rear caliper bolts ~26 lb-ft, anchor ~203 lb-ft [FIELD; VERIFY].
- Rear rotor removal: back off the parking brake shoe **star adjuster** through the access hole if the rotor hangs on the shoes. On a full-floating axle, the rotor slips over the hub studs (verify on truck; some need the hub removed [VERIFY]).
- Parking brake shoes: replace springs and hardware, adjust the shoe diameter with a drum/shoe gauge, then adjust the cable tension at the equalizer per WSM (cable tension release procedure: some Ford trucks require locking the tension spring before cable removal [VERIFY]).

## Bleeding
- Sequence (generic Ford): **RR → LR → RF → LF** (farthest to nearest) [VERIFY WSM]. Pressure bleeder or 2-person pedal method.
- If the ABS HCU was replaced or air entered it: run the **ABS service bleed** routine with the scan tool (IDS/FDRS, FORScan) to cycle the valves.
- **Flush every ~3 years.**

## Hydro-Boost diagnosis
| Symptom | Cause |
|---|---|
| Hard pedal at idle, normal when revving | Weak power steering pump, belt slip, low MERCON LV, restricted lines |
| Pedal pulses/"chatters", hissing at the booster | Internal booster leak / spool valve; aerated fluid |
| No reserve stops with the engine off | **Accumulator** leaking (internal), so replace the booster |
| PS fluid leak at the booster | Booster seals; replace the booster assembly (input rod seal) |
| Self-applying brakes | Booster spool sticking, or return line restricted |
- **Test:** engine off, pump the pedal 5+ times to discharge the accumulator. Hold firm pressure and start the engine: the pedal should drop slightly then firm up. Engine off: the accumulator should give 2–3 assisted applications.
- **Replacement:** discharge the accumulator first (pump the pedal engine-off). Unbolt the master cylinder from the booster without opening its lines when possible (move it aside). Disconnect the 3 hydraulic lines (pump in, steering gear out, return) and the pushrod at the pedal. Bleed by turning the steering lock to lock and pumping the brakes; check for leaks.

## ABS / AdvanceTrac
- Wheel speed sensor DTCs (C0035/C0040/C0045/C0050 etc.): check sensor air gap, tone ring rust-jacking (front unit hub and rear full-float hubs), harness chafe at the knuckles (common in mud/rust states). Use scan data to compare wheel speeds while driving.
- **Steering angle sensor calibration** after alignment or clockspring/column work (scan tool) [VERIFY on 2016 SD].
- **Yaw/roll sensor** calibration after replacing the RCM / restraint module or sensor [VERIFY].
