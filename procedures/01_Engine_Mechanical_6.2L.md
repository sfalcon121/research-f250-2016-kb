# Engine Mechanical — 6.2L 2V SOHC V8 (2016 Super Duty)

Ford WSM reference: **303-01 Engine – 6.2L**. Torque values marked [VERIFY] must be confirmed there. Many 6.2L engine fasteners are torque-to-yield (TTY) and **single-use** (head bolts, often main/rod bolts, flexplate bolts, crank damper bolt) [FIELD]. Always use new TTY fasteners.

## Architecture (know this before you work on it)
- Iron block, deep skirt, cross-bolted main caps [FIELD]. Aluminum heads, **one cam per head (SOHC)**, 2 large valves per cylinder (canted), **roller rocker arms on rocker shafts**, hydraulic lash adjusters in the rockers [FIELD].
- **Dual-plug heads:** 16 spark plugs. Each cylinder has a coil-on-plug unit on the valve cover; the second plug is fed by a short lead [FIELD, verify on truck].
- **Timing drive:** primary chain(s) from the crank to each cam phaser, hydraulic tensioners, chain guides. Variable cam timing solenoids at the front of each head [FIELD]. The engine is **interference** [FIELD]: a jumped chain can contact valves.
- Port fuel injection; composite intake manifold; electronic throttle body; PCV through the RH valve cover baffle.
- Oil pump: crank-driven gerotor in the front cover [FIELD]. Oil filter FL-820-S. Oil pressure sender near the filter/front of the block [VERIFY].

## Compression / leak-down test (dual plug)
1. Warm the engine, disable fuel (pull fuel pump relay or FPDM fuse) and ignition.
2. Remove **both** plugs on the cylinder under test (or all 16 for an accurate crank test). The gauge goes in one hole; leave the other open or plugged per method. For a cranking test, plug the second hole with an old spark plug (no electrode) so you don't read low.
3. Crank with the throttle held open (ETB: hold the pedal to the floor; the PCM opens the throttle in clear-flood mode with the key in RUN).
4. Healthy cylinders read within 10–15% of each other. A single low cylinder with a misfire means a **leak-down test**: air past the intake = intake valve or broken spring; exhaust = exhaust valve; oil fill/PCV = rings; coolant bubbles = head gasket.

## Valve cover removal / gasket / RH baffle (oil consumption)
1. Disconnect the battery. Remove the engine appearance cover and the air intake tube/resonator (note: the resonator interference behind TSB 18-2047 is on the **LH, cyl 5/6** coils).
2. Disconnect the coil connectors, remove coils and secondary leads, the PCV hose (RH) and breather (LH), and the harness clips/brackets. Remove the fuel rail cover if equipped.
3. Remove the valve cover bolts (captured with the gasket). Lift the cover off and clean the sealing surfaces with plastic tools only (aluminum).
4. Inspect the RH cover PCV baffle (2015–2016 oil-consumption concern): oil pooling or a leaking baffle seam means replace the cover with a current Ford part.
5. Apply RTV dots where the front cover meets the head (T-joints), per WSM [VERIFY locations], install a new gasket, and torque bolts in sequence, center outward, to the low WSM spec (~89 lb-in, about 10 Nm) [VERIFY].
6. Reinstall coils with dielectric grease in the boots.

## Broken valve spring: replace on the engine
Symptoms: steady misfire on one cylinder, ticking, low leak-down on the intake or exhaust valve, metal pieces visible under the cover.
1. Remove the valve cover. Rotate the engine so the cylinder is at **TDC compression**.
2. Install an air-hold adapter in a plug hole and apply 90–120 psi shop air. Hold the crank (breaker bar on the damper bolt) because air can rotate the engine.
3. The rocker shaft must come out to reach the spring. Loosen the rocker shaft bolts evenly in sequence [WSM] to relieve load. Note the orientation of each rocker and lash adjuster and **keep them in order**.
4. Use a lever-type spring compressor that bears on the head, then remove keepers, retainer, and spring. Inspect the valve stem seal (replace it while you're there), keepers, and retainer.
5. Install the **current updated Ford spring** (2011–2012 springs were revised) [FIELD]. Compress, install keepers (a dab of grease holds them), and release slowly; tap the retainer with a soft mallet to seat the keepers.
6. Reinstall rockers and shaft in original positions. Torque the shaft bolts in sequence [VERIFY]. Rotate the engine 2 full turns by hand to check nothing binds.
7. Check that the valve isn't bent (leak-down test again). If the valve dropped, the head comes off.

## Exhaust manifold replacement (broken studs/bolts, cracked manifold)
1. Soak the fasteners with penetrant for days if you can. Lift and support the truck; remove the inner fender liner (LH) or the starter/heat shields as needed; disconnect the upstream O2 sensor and Y-pipe flange.
2. Remove the heat shield, then the manifold bolts/studs. Broken stud: if enough remains, **heat with a torch** (aluminum head, so heat the stud, not the head) and use stud pliers or a welded nut. If flush, use a **drill guide jig** for 6.2L manifold flanges (sold as a "6.2L manifold template") and a left-hand drill, then extractor or Time-Sert/Heli-Coil.
3. Clean the head flange flat; check the manifold for warp/crack (straightedge).
4. New gasket (multi-layer steel), new studs/bolts. Torque in sequence from the center outward in 2 passes [VERIFY spec, WSM 303-01]. Reconnect, then run and check for leaks (tick on a cold start).

## Intake manifold removal (for knock sensors, injectors, rear coolant passages, etc.)
1. Relieve fuel pressure (FPDM fuse out, crank 10 s), disconnect the battery, remove the air intake and ETB connector.
2. Disconnect the fuel supply line at the rail (spring-lock tool), the PCV hoses, the vacuum lines (brake booster supply manifold, EVAP purge), and harness connectors (injectors, MAP/TMAP, ETB, VCT solenoids as routed).
3. Remove the intake bolts, then lift the manifold with the fuel rail and injectors. Cover the ports.
4. New intake gaskets (silicone, re-usable only if undamaged), torque in sequence [VERIFY ~ 89 lb-in/10 Nm, then a second pass]. New injector O-rings lubricated with clean engine oil.

## Timing chain / cam phaser / VCT solenoid
Symptoms: rattle at startup lasting 1–3 s, **P0011–P0024 cam timing codes, P0016–P0019 crank/cam correlation**, ticking at the front. Check first: correct oil (5W-30), oil level and pressure, VCT solenoid screens and connectors, solenoid resistance (~7–12 Ω [VERIFY]).
Outline (front cover off; many technicians pull the engine on 4x4 Super Duty, or at minimum remove the radiator/fan shroud):
1. Drain coolant and oil; remove fan/fan clutch and shroud, drive belt, accessory brackets (alternator, PS pump, A/C compressor kept charged and tied aside), water pump, crank damper (**new bolt**, use holder), and front cover.
2. Set the engine at **TDC #1** with the timing marks aligned and use the **Ford cam holding tools** (Ford special tools for the 6.2L camshafts) [VERIFY tool numbers in WSM]. Never rotate cams independently.
3. Compress and pin the tensioners, then remove the chains, guides, and phasers. Phaser bolts are often **single-use** [VERIFY].
4. Install new chains, guides, tensioners, and phasers with the colored links/marks aligned per WSM. Torque phaser bolts with the cam held by the flats (never against the chain).
5. Rotate the engine 2 turns by hand; recheck marks. New front cover gaskets/RTV per WSM bead size. New front crank seal.
6. After assembly: **KAM reset / misfire monitor (CKP) relearn** with the scan tool; check for VCT codes after a road test.

## Cylinder head removal (head gasket / valve job): outline
1. Intake manifold, exhaust manifold, valve cover, rocker shafts/rockers (keep in order), timing components as required for that bank (cam phaser disconnected from chain, chain held with a wedge or tool).
2. Head bolts are **TTY**: remove in reverse of the tightening sequence. Check the block deck flatness and the head for warp. Machine-shop the head: valve job, guides, seals, **all springs** replaced with the current part.
3. New MLS gasket on clean, dry surfaces; **new head bolts**, oiled per WSM. Typical Ford TTY sequence: stage torque, then angle stages, from the center outward [VERIFY exact stages in WSM 303-01; don't guess].
4. Reassemble timing to marks, rotate by hand, refill, and bleed coolant (see cooling).

## Rear main seal / oil pan
- The rear main seal is a one-piece seal in a retainer. The transmission and flexplate must come out (see the 6R140 doc; **grease the converter pilot hub and verify dowels**, SSM 47976).
- Oil pan: on 4x4 the front axle and crossmember are in the way. Many technicians raise the engine on mounts after unbolting them (fan shroud off to protect the fan). Use new gasket/RTV at the front cover and rear seal retainer joints.

## Rebuild notes [FIELD]
- Common rebuild parts: Ford/Mahle/Clevite bearings, Ford rings, **updated valve springs**, chains/guides/tensioners/phasers, oil pump, new TTY bolts, water pump, thermostat, all gaskets. Machine-shop the heads (aluminum) and inspect the rocker shafts and rollers.
- Measure: bore taper/out-of-round, piston-to-wall, main/rod clearances (Plastigage or mic), crank end play, cam journal clearance in the head (SOHC journals are in the head and caps). Get factory clearances from WSM 303-01 Specifications; don't use generic Ford V8 numbers.
- Ford long blocks (Motorcraft reman / new "service engine") are commonly used instead of rebuilding.
- After installing an engine or PCM: program the **engine serial number** if the PCM is replaced (P264F, SSM 47823) and do the **misfire monitor (CKP) relearn**.
