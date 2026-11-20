# Steering & Suspension — including "Death Wobble" (2016 F-250 4x4)

WSM: 204-00 suspension general/alignment, 204-01 front, 204-02 rear, 211-00/02/03 steering. Torques in `02_Specifications_Fluids_Parts_Torque.md` are mostly [FIELD/VERIFY].

## Layout
- **Front:** solid axle, two **radius arms** (bushings at the frame end, two-bolt to axle), **coil springs**, **track bar** (frame bracket on the driver side to axle on the passenger side, or vice versa [VERIFY]; ball-joint end at the axle on 2011+ [FIELD]), stabilizer bar and links, two shocks, **steering damper** on the tie rod/drag link.
- **Steering:** recirculating-ball gear on the LH frame rail, **pitman arm**, **drag link** to the RH knuckle/tie rod, **tie rod** knuckle-to-knuckle with adjusting sleeve. Hydraulic pump (MERCON LV [OM]) also feeds **Hydro-Boost**.
- **Rear:** leaf springs (optional overload/2-stage), shocks, staggered or standard. TSB 15-0117 covers trucks sitting lower in the rear with light loads.

## Death wobble: definition and causes
Violent, self-sustaining oscillation of the front axle/steering after a bump, usually at 40–60 mph, stopping only when you slow way down. A **steering damper only suppresses it**; find the loose part.
**Ranked causes [FIELD]:**
1. **Track bar**: worn ball joint at the axle end, worn bushing at the frame end, **loose track bar bolts** (if the bracket holes egg-shape, the bracket needs replacing), frame bracket cracks.
2. **Ball joints** (upper/lower) and the upper adjuster sleeves.
3. **Tie rod / drag link ends**, adjusting sleeves loose.
4. **Steering gear mounting** bolts loose, sector shaft play, pitman arm nut loose.
5. **Tires**: out of balance, out of round, separated belt, uneven pressure (common trigger after new tires).
6. **Low caster** (lifted trucks, or worn radius arm bushings), bad toe.
7. Wheel bearings with play; radius arm bushings.
8. Weak damper or shocks (contributor, not root cause).

## Death wobble inspection: the "dry steer" test
1. Truck on the ground, engine running (power steering), helper rocks the steering wheel back and forth rapidly about ±1/4 turn without moving the tires much.
2. With a flashlight, watch and **feel** every joint: track bar both ends, drag link ends, tie rod ends, pitman arm, steering gear mounts (watch the box move on the frame), ball joints. **Any lash (one side moves before the other) = worn.**
3. Then lift the front by the frame and check wheel bearings and ball joints (12/6 o'clock play), and spin the tires for runout and balance.
4. Check the steering box sector shaft play: watch the pitman arm vs. the input shaft.

## Track bar replacement
1. Truck **on the ground** (or the axle supported at ride height) so the bolt holes align. Remove the axle-end nut; separate the ball joint taper with a pickle fork or tie-rod puller.
2. Remove the frame-end bolt. Install the new bar (OE Ford or heavy-duty aftermarket: adjustable bars allow re-centering the axle on lifted trucks).
3. **Torque with the weight on the wheels:** frame bolt ~406 lb-ft, axle nut ~184 lb-ft [FIELD; VERIFY]. **Retorque after 100 mi.** Check bracket hole condition.
4. Re-center the steering wheel / check alignment.

## Tie rod / drag link
- Measure the overall length before removal (or count turns). Separate tapers with a puller. New ends: torque castle nuts to spec, then tighten (never loosen) to align the cotter pin.
- Adjuster sleeve clamps ~41 lb-ft [FIELD]. Set toe on an alignment rack.
- Steering wheel off-center after work: adjust at the drag link sleeve, **not** by moving the wheel on the column (clockspring!).

## Steering damper
- Replace if leaking, if it pushes back unevenly, or as part of a wobble fix (not as the only fix). Torques ~66 lb-ft (drag link end), ~59 lb-ft (frame bracket) [FIELD; VERIFY 2016].

## Pitman arm / steering gear
- Pitman arm: puller required. Nut ~350 lb-ft [FIELD; VERIFY]. Align the master spline.
- Steering gear replacement: disconnect the intermediate shaft (mark it; center the steering wheel and **lock it** to protect the clockspring), pressure and return lines (catch MERCON LV), and frame bolts (high torque; [VERIFY]). Bleed the steering after (below).
- **Sector shaft adjustment (lash)** is possible on the gear but over-tightening causes binding. Prefer replacement for wobble/wander due to gear wear.

## Power steering bleed (MERCON LV) [OM + FIELD]
1. Fill to MAX (cold). Front wheels off the ground. With the engine **off**, turn lock to lock ~10–20 times, topping off.
2. Start the engine, turn lock to lock slowly, and top off. Use a vacuum bleed cap on the reservoir (Ford/aftermarket) if it stays foamy. Hydro-Boost shares the fluid: **pump the brake pedal** several times with the engine off/on to bleed the booster.
3. OM check: engine idling, turn left/right several times, engine off, check between MIN/MAX.

## Coil springs, shocks, radius arms
- **Front coil spring:** support the axle with jacks; remove the shocks, sway bar links, track bar axle end (and possibly the drag link) and lower the axle slowly until the spring is free. **Compressed coil springs store dangerous energy, so lower slowly and use a spring compressor if needed.** Watch brake hoses, ABS wires, and vacuum hub lines for stretch.
- Radius arm bushings: replace when cracked or when caster won't hold. Torque bolts at ride height [FIELD ~222 lb-ft; VERIFY].
- Rear leaf springs: U-bolts are **single-use**; torque in a crisscross pattern per WSM [VERIFY] and retorque after a few hundred miles.

## Alignment
- Caster and camber on the Dana 60-type are set with **upper ball joint offset sleeves (adjusting cams)** [FIELD]; toe at the tie rod sleeve. Caster spec ~ +3° to +5° (more caster is more stable) [VERIFY WSM spec]. Lifted trucks often need caster correction (offset bushings or drop brackets), per the PC-01.12.2016 communication.
