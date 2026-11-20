# Ignition, Fuel and Emissions — 6.2L

## Spark plugs (16 × Motorcraft SP-526, gap 0.041–0.047") [OM]
Interval: 97,500 mi normal; **60,000 mi** for towing, idle, or severe use [OM].
1. Engine **cool to warm**, never hot (aluminum heads). Disconnect the battery. Remove the engine cover and air intake as needed (LH cyl 5/6 behind the resonator).
2. Blow out the plug wells with compressed air (debris falls into cylinders otherwise).
3. Remove the coils (connector tab, single bolt) and the secondary leads to the second plugs. Label everything.
4. Break each plug loose slowly. If it's tight, stop, apply penetrant, wait, and work it in and out in quarter turns.
5. Check the gap on new plugs (adjust only with a proper gap tool; don't pry on the center electrode).
6. Thread in by hand with a rubber hose or extension, then torque **~18 lb-ft (24 Nm) [VERIFY 2016 WSM]**.
7. Put dielectric grease inside the coil boots; inspect boots for carbon tracking and replace any that are cracked. Reconnect the connectors; **make sure the cyl 5/6 connectors don't touch the intake resonator (TSB 18-2047)**.
8. Clear codes and road test.

## Coil diagnosis (misfire P030X, coil primary P0351–P0358)
- Swap the suspect coil to another cylinder; if the misfire follows, the coil is bad.
- **P0355/P0356** on 2014–2016 6.2L: inspect the cyl 5/6 connector/pigtail for an open caused by resonator rubbing (**TSB 18-2047**).
- Check boots for moisture (common after washing the engine). Check the plug well for oil (valve cover gasket or plug tube seal).
- Coil primary: check 12 V feed with key on, PCM control ground pulse (scope), and connector pin fit (drag test).
- If coils and plugs are good and one cylinder still misfires: compression/leak-down (**broken valve spring**), injector balance or noid light, vacuum leak at the intake gasket.

## Fuel system (returnless, FPDM-controlled)
- **Fuel filter: lifetime, in-tank** (part of the pump module); no service [OM].
- Fuel pump driver module (FPDM) commands pump speed from the PCM. FPDM location: on the frame rail/crossmember near the tank [VERIFY]. **Corrosion on the FPDM and its connector is a common Super Duty failure**: no start, stalling, P0627/P0628/P0629, U0109 [FIELD].
- **TSB 16-0060:** P0627, P025A, P025B, U0109 on 6.2L/6.8L built ≤ 4/6/2016 → **PCM reprogram**.
- Fuel pressure test: Schrader on the fuel rail. Spec per WSM (typically 55–65 psi commanded) [VERIFY]. Watch FRP PID versus desired.
- **Fuel pump/sending unit replacement:** drop the tank (35 gal; drain or run low first) or lift the box (crew cab: about 8 box bolts, harness and filler neck; usually faster). Disconnect the battery, relieve pressure, disconnect lines with spring-lock tools, use the lock-ring tool, and install a new seal. Torque tank strap bolts per WSM [VERIFY].
- Injectors: high-impedance top-feed. Check resistance (~11–18 Ω [VERIFY]) and balance-test with the scan tool or a pressure-drop test.

## Air intake / throttle
- MAF sensor in the intake tube. Clean only with MAF cleaner. Inspect the intake tube clamps and resonator for leaks (unmetered air causes **P0171/P0174 lean** codes).
- Electronic throttle body: **don't condemn it from ETC_ACT/ETC_DSD PIDs (SSM 46085)**. Diagnose with DTCs (P2111, P2112, P2135, P2101). Clean coking with throttle body cleaner, key off. After replacement or cleaning, do the **KAM reset and idle relearn** (idle 10 minutes with accessories off, then drive) [FIELD].

## EVAP
- Purge valve on the intake side, canister vent (CVS) at the canister near the tank, Easy Fuel capless filler (no gas cap). **P0455/P0456/P0457**: inspect the capless funnel flapper/seal (clean it, check for debris) and the CVS for mud/spider blockage, then smoke test.

## Catalysts / O2 sensors
- 4 O2 sensors (upstream/downstream each bank). P0420/P0430: check for exhaust leaks (manifold studs!) and misfire history before replacing cats.
- Sensor removal: O2 socket and heat. Use anti-seize only if the new sensor threads aren't pre-coated.

## KAM reset / PCM relearns
- Battery disconnect ~ 1–2 min or **scan tool KAM reset**, then idle relearn and drive.
- **Misfire monitor (CKP) relearn**: required after a PCM, crank sensor, flexplate, or damper change. Ford scan tool or FORScan service procedure, or the drive-cycle method of decels from 60 mph [VERIFY].
- PCM replacement → **PMI with IDS/FDRS** (SSM 51947 order of operations) and **ESN programming (SSM 47823, P264F)**. PATS keys must be relearned (BCM/PCM parameter reset).
