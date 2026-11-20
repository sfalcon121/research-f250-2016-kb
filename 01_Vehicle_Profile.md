# Vehicle Profile — 2016 F-250 Super Duty Lariat 4x4, 6.2L Gas

## Generation context
- **2011–2016 Super Duty (P2 platform).** The 2011 model year introduced the 6.2L gas engine, the 6R140 transmission, and the 6.7L Power Stroke. The steel cab and box carry over from the 2008–2010 bodies. 2016 is the **last year** of this generation; 2017+ trucks have aluminum bodies and different frames and electronics, so **2017+ procedures and TSBs usually do NOT apply**.
- Assembly: Kentucky Truck Plant (Louisville). VIN 11th character = **E**. [VERIFY by VIN]
- Lariat equipment (typical): leather, power/heated/cooled front seats (the climate seat filter FS-104 needs service [OM]), SYNC with MyFord Touch (SYNC 3 arrived in 2017 Super Duty), dual-zone EATC, power-telescoping/folding trailer-tow mirrors (optional), rear-view camera, reverse sensing, optional moonroof, optional 5th-wheel/gooseneck prep, optional electronic locking rear axle.

## Powertrain
| Item | Detail |
|---|---|
| Engine | 6.2L (379 cu in; manual lists 378 [OM]) 90° V8, **SOHC 2 valves/cylinder**, roller-follower rocker arms on shafts, variable cam timing (phaser on each cam), **2 spark plugs per cylinder (16 plugs) fired by 8 coil assemblies** [FIELD], iron block, aluminum heads, port fuel injection, electronic throttle |
| Output (Super Duty tune) | 385 hp @ 5,500 rpm, 405 lb-ft @ 4,500 rpm [FIELD/Ford press] |
| Compression | 9.8:1 [OM] |
| Firing order | 1-5-4-8-6-3-7-2 [OM]. Cylinders 1–4 are the passenger (RH) bank front to rear; 5–8 the driver (LH) bank. |
| Fuel | 87 octane minimum [OM]; flex fuel (E85) on VIN engine code 6 |
| Transmission | **6R140 TorqShift 6-speed** automatic, code **P** [OM]. Ford-built and derived from the 6R80/ZF 6HP26 family. Shift control by the PCM through a valve-body-mounted solenoid body with an internal harness and TFT/speed sensors [VERIFY architecture in WSM 307-01]. Has a **dipstick** (gas trucks) [OM]. Tow/Haul mode, SelectShift |
| Transfer case | Two-speed part-time, chain drive, **electronic shift-on-the-fly (ESOF)** with dash knob (2H/4H/4L) on Lariat [OM]. Aftermarket/reman catalogs call it 1628-type (electric shift, Magna/NVG 273F family) [FIELD]; the manual-lever version is 1128-type. Confirm by the case ID tag. |
| Front axle | Solid Dana 60-type ("Super 60"), coil springs, two radius arms, track bar, steering damper, stabilizer bar. Vacuum-actuated **auto-manual locking hubs** (rotate to LOCK to override) [OM]. Unit hub bearings bolt to the knuckle. |
| Rear axle | Ford (Sterling-design) **10.50"** [OM], **full-floating** [FIELD]; Traction-Lok limited slip or optional electronic locker. Ratios on 6.2L are typically 3.73 or 4.30. Read the axle code on the door-jamb label. |
| Brakes | 4-wheel disc, **Hydro-Boost** (power steering pump driven) [FIELD]; rear parking brake is drum-in-hat. ABS, AdvanceTrac with RSC. |
| Steering | Recirculating-ball gear, hydraulic pump (fluid = **MERCON LV** [OM]), pitman arm, drag link, tie rod; steering damper |
| Fuel tank | 35 gal (pickup) [OM]. **Lifetime in-tank fuel filter**, no service [OM]. Returnless system with fuel pump driver module (FPDM). |
| Electrical | Single battery (BXT-65-650 std / BXT-65-750 opt) [OM]; 157A or 200A alternator [VERIFY]. CAN modules: PCM, BCM (Smart Junction Box), ABS, RCM, IPC, APIM (SYNC), FCIM/FCDIM, TCCM (4x4), etc. |

## Decoding the VIN (17 chars) [OM layout]
- 1–3 World manufacturer (1FT = Ford truck)
- 4 Brake/GVWR class, 5–7 line/series/body (e.g. **W2B** = F-250 4x4 Crew Cab; **X2B** = F-250 4x4 SuperCab) [VERIFY]
- **8 Engine: `6` = 6.2L gas** (`T` = 6.7L diesel, `Y` = 6.8L V10) [FIELD]
- 9 check digit, **10 = G (2016)**, 11 plant, 12–17 serial
- Door-jamb certification label: axle code, transmission code (P = 6R140), paint, build date (essential for TSB applicability).

## Determining build-specific options (do this before ordering parts)
1. Read the door-jamb label for build date, axle code, and transmission code.
2. Enter the VIN at parts.ford.com, or a Ford dealer parts catalog, for exact part numbers.
3. Window sticker: Ford owner sites can retrieve it by VIN.
4. Check the axle tag on the rear diff cover bolt for ratio and limited-slip/locker status.
5. Check the transfer case ID tag on the rear case half.
