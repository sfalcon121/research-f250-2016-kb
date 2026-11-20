# Electrical, Network, Body, HVAC and SRS — 2016 F-250 Lariat

WSM: 412 climate, 413 instruments, 414 charging, 415 audio/SYNC, 417 lighting, 418 module communications, 419 anti-theft/PATS, 501 body, 501-20B SRS.

## Fuse and relay locations [OM]
- **Power Distribution Box (BJB)** under the hood on the driver side: high-current fuses and relays (starter, fuel pump/FPDM, PCM power, A/C clutch, horn, ABS, trailer tow, blower).
- **Passenger compartment fuse panel / Smart Junction Box (BCM)**: in the passenger footwell kick panel / lower dash [VERIFY]. The fuse charts with full fuse/relay numbers and ratings are in the OM text (`sources/ford_official/*readingorder.txt`, search "FUSE SPECIFICATION CHART").
- Upfitter switches (Lariat option): auxiliary circuits AUX1–AUX4 with relays and wires to the engine compartment [OM].

## Network (CAN) basics
- **HS-CAN:** PCM, ABS, RCM, IPC, TCCM, PSCM if equipped, BCM gateway, etc. **MS-CAN:** HVAC, APIM (SYNC), audio, FCIM/FCDIM, DDM/PDM (door modules), memory seat module, etc. [VERIFY exact module assignment by VIN].
- **No communication / multiple U-codes:** check the battery, grounds, then DLC pins 6/14 (HS-CAN) and 3/11 (MS-CAN). Resistance ~60 Ω key-off between the CAN+ and CAN- pins on a healthy bus with both terminators. Disconnect modules one at a time to find a shorted one.
- **SSM 45894** (2016 SD built ≤ 5/1/2016): inoperative blower, power-fold mirror, RKE, or no MS-CAN communication.
- **SSM 46236**: flickering panel lights with a plow/winch → BCM reprogram.

## Battery / grounds
- See the cooling/charging doc and **SSM 47886/48123** (replace the corroded positive clamp only).
- Main grounds: battery-to-engine, engine-to-frame strap, body ground near the battery/fender. Voltage-drop test under load.

## PATS / keys
- 2016 SD Lariat: PATS transponder key or **Intelligent Access (push-button) if equipped [VERIFY]**. With 2 programmed keys, a third can be self-programmed by the owner using the OM procedure; otherwise the scan tool is needed (security access).
- **SSM 47824:** "Error 232: Key Table Not Allocated" during programming → **replace BCM**.

## Common electrical / body problems [FIELD]
| Issue | Notes |
|---|---|
| **Blend door actuator clicking** in the dash | Dual-zone EATC actuators fail; replace (some are behind the glovebox, some need dash access). Run HVAC self-test/actuator calibration after (cycle the key or EATC diagnostic mode). |
| Blower works only on high, or not at all | Blower motor resistor/control module (with connector melt), blower motor |
| A/C weak, **P06A0** | **SSM 47850**: EVDC compressor control valve, test with Rotunda 339-EVDC100 [VERIFY that the 6.2L compressor is EVDC]. Check charge **29 oz R-134a** [OM] by weight, after evacuation. |
| Clockspring: horn/cruise/airbag light | **Recall 22V337 / 22S35**. Free replacement. |
| Backup camera blank | **Recall 25V572 / 25S89** |
| SYNC/MyFord Touch glitches, Bluetooth | **SSM 46092**, APIM updates; master reset; SiriusXM issues (**SB-45316**) |
| Power-telescoping mirror failures | Motor/glass actuator, mirror heater connector corrosion, see SSM 45894 (MS-CAN) |
| Tailgate handle/cable/latch and lock rods | Rods/clips break; replace the latch/rods |
| Door lock actuators | Fail with age; replace the latch assembly (actuator integrated) |
| Cab corners, rocker panels, rear wheel arches, tailgate bottom | **Rust (steel body)**. Check before buying or repairing. Running boards can damage sills off-road (**SSM 45900**). |
| Water leaks (3rd brake light, rear slider window, moonroof drains) | Reseal the brake light gasket; clear the moonroof drain tubes |

## SRS (airbags) — safety rules
1. **Disconnect the battery negative and wait at least 1 minute** (WSM specifies the backup power depletion time [VERIFY]) before touching any SRS component, clockspring, or steering wheel.
2. Never probe airbag connectors with a test light or ohmmeter. Store live airbags facing up. Use the scan tool to read RCM DTCs (**B141B/B141C**, TSB160001).
3. **Clockspring:** center the steering (wheels straight), lock it, and don't rotate an unlocked clockspring. Replacement clocksprings come pinned in center.
4. After SRS repairs: clear DTCs, check the airbag lamp prove-out. Some RCM replacements need PMI/configuration.

## HVAC service
- R-134a **29 oz**, PAG **YN-12-D**, system oil **4.2 fl oz** [OM].
- Compressor replacement: replace the receiver/accumulator (or desiccant) and orifice tube/TXV [VERIFY system type]. Flush the condenser if there was a debris failure; add oil per WSM distribution. Evacuate ≥30 min, then charge by weight.
- Heater core: dash-out job (largest labor op); first try flushing for a no-heat complaint (also bleed the coolant system).
