# 6R140 TorqShift 6-Speed Automatic — Service, Diagnosis, Rebuild

WSM: **307-01 Automatic Transmission – 6R140**. Fluid: **MERCON LV only** (XT-10-QLVC) [OM]. Dry fill **16.7 qt (15.8 L)** [OM]. Filter **BC3Z-7A098-B** (6.2L) [OM]. Scheduled change: **105,000 mi** normal [OM]. Technicians recommend 30–60k when towing [FIELD].

## Design overview [FIELD]
- Ford-designed heavy-duty derivative of the 6R80 (itself ZF 6HP26-based architecture): Lepelletier gearset (single front planetary plus rear Ravigneaux), **5 friction elements** (clutches A, B, E; brakes C, D) plus a one-way clutch in 1st (non-towing) [VERIFY element naming].
- Solenoid body and TCM functions on the valve body (main control, 7A100). Shift solenoids SSA–SSE, TCC solenoid, line pressure control (LPC). Turbine and output shaft speed sensors and TFT sensor are on the internal harness.
- Gas 6.2L units use a different torque converter and calibration than diesel; parts aren't always interchangeable.
- **Coast clutch / "P0751/P0730/P2700"** pattern on early builds (TSB 16-0057, built ≤ 12/15/2015).

## Fluid level check (Ford procedure) [OM]
1. Drive ~19 mi (30 km) to normal temperature; the cluster trans temp gauge is in the normal range.
2. Level ground, parking brake on, engine **running**, foot on brake; move the lever through every range, pausing in each.
3. Park, engine running. Pull the dipstick, wipe, fully reseat, pull and read.
4. **Correct reading at 196–215°F (91–102°C)** is in the hot-range crosshatch. Add in **8 fl oz (250 mL)** increments through the filler tube. Overfill causes aeration, shift/engagement problems and damage. Don't drive if there's no fluid on the stick and ambient is above 50°F.
5. Use a scan tool TFT PID to confirm temperature rather than guessing.

## Pan drop, filter and refill
1. Hot fluid warning. Lift the truck level. Drain the pan drain plug (if equipped) or loosen pan bolts on one side to tip the pan. Expect ~7–8 qt out [FIELD].
2. Remove the pan (bolts ~80 lb-in/9 Nm [FIELD]); clean the magnet(s) and inspect the debris. **Fine gray paste is normal; brass/bronze glitter, steel chunks, or friction material flakes indicate wear.**
3. Pull the filter straight down (it has a seal in the valve body bore; make sure the old seal came out). Lubricate the new filter seal with ATF and push it fully home.
4. New pan gasket (reusable molded on some pans [VERIFY]); torque pan bolts in a crisscross. Drain plug ~20 lb-ft [FIELD; VERIFY].
5. Refill through the dipstick tube with MERCON LV (approximately what came out), then set the level **hot** per the procedure above.
6. Optional: **adaptive (KAM) transmission reset** with the scan tool only if shift quality complaints were the reason. Normally keep the learned adaptives after a routine service.
7. Repeat a drain-and-fill 2–3 times to approach a full exchange (no machine flush unless it uses MERCON LV only; Ford allows flushing with the same new fluid [OM]).

## DTC / symptom diagnosis
| DTC / symptom | Check |
|---|---|
| **P0751** SSA performance / stuck off, **P0730** incorrect ratio, **P2700** friction element apply time | **TSB 16-0057**: on builds ≤ 12/15/2015, PCM reprogram first. Then check line pressure, the solenoid body, and the coast clutch per TSB. |
| P0711–P0713 TFT | Internal harness / TFT sensor (on solenoid body) |
| P0715/P0717 TSS, P0720/P0722 OSS | Sensor/internal harness/connector at case (bulkhead); fluid leak at the case connector wicking up harness |
| P0741 TCC slip / shudder at 40–55 mph | Fluid condition and level; TCC solenoid; converter clutch; reprogram; worn converter |
| P0960–P0977 solenoid circuit | Case connector, internal harness, solenoid body |
| Harsh 2–3 / 3–4, flare | Level, adaptive reset/relearn, valve body bore wear (**SSM 46451**: valve body overhaul inspection), solenoid |
| No reverse / delayed engagement | Level, pump, clutch pack, valve body |
| **Fluid leak at the case or pan crack** | **TSB 22-2356**: rear driveshaft imbalance cracks the case/pan → replace the rear driveshaft and repair the case/pan |
| Leak at front | Converter hub seal / pump seal; check the rear main seal (engine oil vs. red ATF) |
| Leak at cooler lines | Quick-connect O-rings at the case and radiator; corroded steel lines (rust belt) |

## Transmission removal / installation (4x4) — outline
1. Disconnect the battery. Lift and support. Drain ATF. Remove the front and rear driveshafts (index-mark them; **check the rear driveshaft balance**, TSB 22-2356). Remove the transfer case (separately, with a transmission jack; ~100 lb).
2. Remove the exhaust Y-pipe as needed, starter, cooler lines (disconnect tool), case connector, TR sensor/shift cable, vent hose, dipstick tube.
3. Remove the inspection cover; remove the **torque converter nuts** (rotate the crank).
4. Support the engine (rear of the block), remove the crossmember/mount, and the bell housing bolts. Pull the transmission straight back with the converter retained.
5. Install: **lubricate the converter pilot hub with XL-5-A grease (SSM 47976)**, confirm **dowel pins** in the block. Fully seat the converter (it should be recessed in the bell housing; on a bench, measure per WSM). Draw the transmission in with the bell bolts only when it's flush; never pull it in with the bolts. Torque converter nuts and bell bolts per WSM [VERIFY].
6. Refill, set the level hot, clear the adaptives, and drive-cycle relearn. Program the PCM if a new transmission or solenoid body comes with a strategy update or a **solenoid characterization file**: new solenoid bodies/valve bodies on 6R units can require downloading the **strategy/calibration ID or Solenoid ID from the tag** with the Ford scan tool [VERIFY 6R140 requirement].

## Rebuild guidance [FIELD]
- Common failure points: **coast clutch** (P0730/P0751), **intermediate/input shaft bushing and sealing ring wear** causing pressure loss, **torque converter** (shudder), high-pressure **pump**, **valve body bore wear** (ZF-style; use oversized valve kits / Sonnax), clutch packs from heat when towing.
- Rebuild kit should include a Ford/OE friction and steel set, sealing rings, bushings, pump seal, filter, pan gasket, latest-revision solenoids and sensors. Check the **intermittent neutral** issue (Sonnax tech note on 6R140 elusive neutral), often a sealing or valve body issue.
- Converter: rebuild or replace with the correct gas-engine converter; flush/replace the **cooler** (or install an inline filter) after any internal failure.
- After a rebuild: clear adaptives, follow the WSM drive cycle, and confirm with scan data (TCC slip, shift times).

## Shift cable / TR sensor
- Column shift. Adjust the cable at the transmission with the lever in Park/Drive per WSM. The TR (range) sensor sets P/N start; misadjustment causes no-start in Park or wrong PRNDL display.
