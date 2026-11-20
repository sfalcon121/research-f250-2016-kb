# Cooling, Accessory Drive, Charging and Starting — 6.2L

## Cooling system facts
- Capacity **21.3 qt (20.2 L)**, **Motorcraft Orange VC-3DIL-B** prediluted [OM]. First change at 105k / 6 yr, then every 45k / 3 yr [OM].
- Components: belt-driven water pump (front cover), thermostat housing at the front of the intake/water crossover [VERIFY location], **viscous fan clutch** (mechanical or electronically controlled; check for a wiring connector at the clutch [VERIFY]), aluminum radiator with plastic tanks, degas (pressurized) reservoir, engine oil cooler, transmission cooler in the radiator plus an auxiliary transmission cooler, heater core.

## Drain, fill and bleed
1. Engine cold. Remove the degas cap. Open the radiator draincock (lower LH/RH tank) and drain into a clean pan. Some technicians also pull the lower hose for more volume.
2. Close the drain. **Vacuum fill (Airlift) is recommended** because it avoids air pockets in the heater core. Otherwise fill slowly through the degas bottle to the MAX line.
3. Set the heat to MAX, blower low. Run the engine at ~2,500 rpm for a few minutes, then idle and top off. Let it reach operating temperature until the thermostat opens (upper hose hot); top off after cool-down. Recheck the level cold over the next few drives.
4. Pressure test the system and cap (cap rating stamped on the cap; ~ 16–20 psi [VERIFY]).

## Water pump replacement (outline)
1. Drain coolant; remove the fan shroud and the **fan/fan clutch** with a fan-clutch wrench set. **Check the thread direction and whether the clutch is electronically controlled (connector at the clutch) in WSM 303-03** before applying force [VERIFY].
2. Remove the drive belt (tensioner: rotate with a breaker bar/belt tool) and the water pump pulley.
3. Unbolt the pump; clean the gasket surface (aluminum, plastic scraper). New gasket/O-ring; torque bolts evenly in a crisscross [VERIFY spec].
4. Reinstall pulley, belt (check routing on the label / OM p.303), fan clutch, shroud. Refill and bleed.

## Thermostat
- Symptoms: overheating, or temperature never reaching normal, low heat, **P0128**.
- Replace the thermostat and gasket together; orient the jiggle valve/bleed upward. Refill/bleed.

## Overheat diagnosis order
Coolant level and leaks → fan clutch engagement (hot engine: the fan should roar on a hot start and be hard to spin when engine off and hot) → radiator externally plugged (A/C condenser/trans cooler stack, bugs) → thermostat → water pump impeller and belt slip → head gasket (combustion leak test, bubbles in the degas bottle, CO2 test kit) → towing loads (watch ECT and trans temp).

## Accessory drive belt
- Inspect every 15k after 105k; replace at 150k [OM]. Check the tensioner arm for wobble/noise and the idler pulley bearings (spin by hand with the belt off).
- Routing: underhood label / OM "Drivebelt Routing 6.2L" (E163761).

## Charging system
- Alternator: belt-driven; output **[VERIFY 157A or 200A by RPO]**. Battery BXT-65-650 (std) or BXT-65-750.
- Test: battery OCV ≥12.6 V. Running at idle 13.5–15.0 V (Ford uses **smart charge**, so voltage varies with the PCM command). Carbon-pile or conductance test the battery first.
- **Positive battery clamp corrosion (SSM 47886)**: replace the clamp BT4Z-14450-AA, crimp and heat shrink, don't shorten the cable. Clean the ground straps (engine-to-frame and body ground). Corroded grounds cause many "electrical gremlins".
- Battery replacement: if equipped with a **Battery Monitoring Sensor (BMS)** on the negative cable, do the BMS reset with the scan tool, or wait 8 h with the key off [VERIFY if equipped on 2016 SD].

## Starting system
- No-crank: battery and cable voltage drop test (cranking: <0.5 V drop each side), starter relay in the BJB, PATS indicator (flashing = key/transponder issue; **SSM 47824: key programming fails "Error 232" = replace BCM**), Park/neutral signal (TR sensor at the transmission).
- Starter replacement: on the RH or LH side of the transmission bell housing [VERIFY side]. Disconnect the battery, remove the heat shield/cable nut, then the 2–3 mounting bolts. Torque mounting bolts per WSM [VERIFY].
