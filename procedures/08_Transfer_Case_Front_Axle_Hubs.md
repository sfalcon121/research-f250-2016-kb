# Transfer Case, 4x4 Controls, Locking Hubs and Front Axle (Dana 60-type)

WSM: 308-07 transfer case, 205-04 (or 205-03) front drive axle [VERIFY numbering], 204-01 front suspension/hubs.

## How the 4x4 works on this truck [OM]
- **ESOF knob**: 2H / 4H / 4L. 4H can be selected on the move (under ~55 mph [VERIFY]); 4L requires a stop and Neutral.
- **Auto-manual hub locks:** in AUTO, the transfer case control module (TCCM) applies **engine vacuum** through a hub-lock solenoid and lines to the knuckles to lock both hubs when 4x4 is selected. Turning the hub dials to **LOCK** mechanically engages the hubs (override). Remove the wheel center ornaments to reach the dials [OM]. **Both hubs must be in the same position.**
- 4L engaged = "4x4 LOW" indicator; electronic locker (if equipped) works in 4L or as programmed [OM].

## Fluids
- Transfer case: **2.0 qt XL-12** [OM]. Change at 60k for towing/dust/off-road (30k for extended idle) [OM]. Fill to the bottom of the fill hole.
- Front axle: **3.0 qt 80W-90** XY-80W90-QL [OM]. Change after water submersion [OM].
- Spindle bearing grease: **XG-11** [OM].

## Transfer case fluid change
1. Level truck. Remove the **fill plug first** (so you know you can refill), then the drain plug. Clean the magnetic drain plug.
2. Reinstall the drain plug (new sealant/washer per WSM; torque [VERIFY]). Fill with XL-12 until fluid dribbles from the fill hole (~2.0 qt). Install the fill plug.

## Transfer case problems
| Symptom | Likely cause |
|---|---|
| 4x4 indicator flashes, won't shift | **Shift motor / encoder** (on the case; corrosion at the connector), TCCM, mode switch, low battery voltage. TCCM DTCs (P1xxx/C/U) with scan tool. Shift motor can be replaced without removing the case. |
| Grinding/whine in 4x4, or chain slap noise | Stretched chain, front output bearing wear, low fluid |
| Fluid leaks | Front/rear output seals, shift motor shaft seal, case halves (RTV) |
| Front driveshaft spins in 2H | Hubs stuck locked or dragging. Normal: the front driveshaft doesn't spin in 2H with hubs free. |
- **Rebuild:** master overhaul kits for this case are sold as **NV273F (2011–2016 SD, slip-yoke or fixed-yoke rear)**. They contain bearings, seals, and chain. Reman units are listed as 1128 (manual) / **1628 (electric shift)** type [FIELD]. Check the ID tag on the case.

## Auto hubs not locking: diagnostic flow [FIELD]
1. Turn both hubs to **LOCK** and shift to 4H. If the front now drives, the problem is the vacuum/auto system, not the transfer case.
2. **Vacuum lines:** inspect the rubber/plastic lines from the solenoid down to each knuckle. Pull gently on them; brittle lines crack at bends near the knuckle. Cap off one side at a time to isolate the leak.
3. **Vacuum test:** a vacuum gauge on the hub supply at the solenoid output with 4x4 commanded should pull and **hold ≥10 inHg for ~45 s** [FIELD quoting WSM; VERIFY].
4. **Hub lock solenoid:** connector seated (broken locking tab is common), power/ground commanded by the TCCM; solenoid clicks and passes vacuum.
5. **Knuckle/spindle vacuum seals:** if the line holds vacuum but the hub circuit leaks down, the **spindle (knuckle) vacuum seals** or hub internal seals are leaking (dust/mud accelerates this; SSM 46345 knuckle seal shield kit GC3Z-54024A38-A).
6. **Hub body:** the hub assembly can fail internally (worn clutch ring, broken tabs). Replace it as an assembly.

## Front hub and wheel bearing replacement (unit bearing) — outline
1. Loosen the lugs, lift and support, remove the wheel. Remove the brake caliper (hang it, don't strain the hose) and the **caliper anchor bracket** (new bolts usually required [VERIFY]), and the rotor.
2. Remove the locking hub assembly (screws/bolts from the outside on auto-manual hubs [VERIFY design]) and the **axle shaft nut/retainer**.
3. Disconnect the ABS wheel speed sensor and the vacuum line from the knuckle.
4. Remove the hub-bearing-to-knuckle bolts (from the back of the knuckle). Rust-welded hubs: use penetrant and a slide-hammer hub puller; don't hammer on the bearing.
5. Clean the knuckle bore and mating face thoroughly (rust jacking causes bearing failure and runout). Light anti-seize on the bore (not the faces) [FIELD].
6. Install the new hub with new vacuum seals/O-rings and torque bolts to WSM [VERIFY: no reliable published 2016 value found]. Reinstall axle nut and hub lock. Torque the caliper bracket and caliper. Check the ABS sensor gap and connector.
7. Test: spin and check play; road test; test the vacuum hub engagement.

## Front axle U-joints, axle shafts, spindle bearings, seals
- Symptoms: clunk/bind when turning in 4x4, vibration in 4x4, grease on the knuckle, **wheel bearing growl**.
- Procedure outline: hub assembly off (above) → remove the spindle bolts/nuts, tap off the spindle → pull the outer axle shaft/U-joint assembly out → replace the U-joint (press; Spicer 1410/1480 series [VERIFY]), **spindle needle bearing (grease with XG-11)**, and the spindle seal and **vacuum seals**. Inspect the inner axle shaft seal at the diff tube.
- Spindle-to-knuckle nuts commonly listed at ~65 lb-ft [FIELD; VERIFY].

## Ball joints
- Check: lift by the axle tube or under the lower ball joint; pry the bottom of the tire vertically with a bar while watching the joint; check for horizontal play with the wheel at 12/6 o'clock (not 3/9, which is tie-rod). Wear spec is per WSM (Ford usually allows very little or none on Dana 60 [VERIFY]).
- Replace upper and lower with a **ball joint press** (Dana 60 adapter set). Knuckle off the axle: tie rod end, ABS wire, caliper bracket, hub, and spindle as needed, then the ball joint nuts. Replace with greasable heavy-duty joints if wanted. Upper joints often have a camber/caster adjusting sleeve (orientation sets alignment). **Mark its position or get an alignment after.**
- Torque the upper ball joint nut ~69 lb-ft (then tighten to cotter pin alignment, never loosen) [FIELD; VERIFY]; lower per WSM [VERIFY].

## Front differential
- Leak at the pinion seal or diff cover; whine on decel (pinion bearing preload); clunk (backlash, worn spider gears).
- Gear setup on a Dana 60-type: shim-type pinion depth, **crush sleeve or shim-pack preload** per WSM [VERIFY], backlash ~0.005–0.008" typical [FIELD; VERIFY], read the gear pattern with marking compound. This is a specialist job, so recommend a driveline shop unless the user has the tools (dial indicator, inch-pound torque wrench, bearing pullers, case spreader for Dana).
