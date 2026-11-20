# Sources, Known Gaps, and How to Expand This Knowledge Base

## Primary sources included
| Source | File(s) | Notes |
|---|---|---|
| Ford 2016 Super Duty Owner's Manual, 2nd printing (Aug 2015), official PDF from fordservicecontent.com | `sources/ford_official/2016-F-250-350-450-550-Owners-Manual-version-2_om_EN-US_08_2015.pdf` (+ layout and reading-order text) | Capacities, fluids, Motorcraft parts, maintenance schedule, fuse charts, 4x4/hub operation, towing, TPMS, warning lights |
| Ford 2016 Super Duty Quick Reference Guide | `sources/ford_official/2016-SuperDuty-QRG-...pdf` | |
| NHTSA Manufacturer Communications (TSB) flat files 2010–2024 | `sources/nhtsa/tsbs_2016_superduty.json` → `04_TSBs_SSMs_full_list.md` | 227 Ford bulletins indexed to the 2016 F-Super Duty, with applicability and engine flags |
| NHTSA complaints flat files 2015–2026 | `sources/nhtsa/complaints_2016_f250.json` → `08_NHTSA_Complaint_Patterns.md` | 291 unique complaints |
| NHTSA recalls API and flat file | `sources/nhtsa/recalls*.json` → `04a_Recalls.md` | 4 campaigns |
| Web research (technician forums, rebuilder notes, aftermarket instructions) | Folded into the docs with **[FIELD]/[VERIFY]** tags | e.g. ford-trucks.com, Sonnax 6R140 note, Gears Magazine 6R140 article, Diesel Hub axle service pages, aftermarket pan/track bar instructions |

## Known gaps (and why)
1. **Ford Workshop Manual (WSM), PC/ED diagnostic manual, and wiring diagrams** are copyrighted and sold through **motorcraftservice.com**. They aren't included. This is the single biggest gap: exact torque sequences, internal clearances, pinpoint tests, connector pinouts.
2. **Full TSB PDFs:** NHTSA hosts many at `https://static.nhtsa.gov/odi/tsbs/<year>/MC-<odi_id>-9999.pdf` (or `-0001.pdf`). Bulk download was **blocked** in this build because NHTSA's server rejects non-browser clients. The summaries and IDs are in `04_TSBs_SSMs_full_list.md`. You can download the PDFs one by one in a browser (or with your approval for a scripted download) and drop them in `sources/nhtsa/tsb_pdfs/`.
3. Some torque values are **[VERIFY]** because public sources conflict.
4. Labor times and exact Ford part numbers per VIN (use parts.ford.com with the VIN).

## How to expand (staying under 2.5 GB; current size is ~14 MB)
| Add | How | Size estimate |
|---|---|---|
| **Ford WSM + wiring + PC/ED for 2016 F-Super Duty** | Buy a short-term **PTS subscription at motorcraftservice.com**. Save the sections you need as PDF (print to PDF) for **personal use**. Check the license terms before loading them into an AI tool. | 300–900 MB as PDF; ~50–150 MB as text |
| All TSB PDFs listed in `04_TSBs_SSMs_full_list.md` | NHTSA site, by bulletin, or ask Claude to script the download with your permission | ~50–150 MB |
| Haynes/Chilton **"Ford Super Duty F-250/F-350 2011–2016"** (gas & diesel) | Buy the book or online version; DIY-level procedures with torque | ~100 MB as a scan |
| ALLDATA DIY / Mitchell1 ProDemand DIY (eautorepair) | Single-vehicle subscription; export procedures you use | variable |
| 6R140 rebuild manual (ATSG 6R140) | Purchase from ATSG | ~30 MB |
| Dana 60 / Ford 10.5 gear setup guides | Spicer (Dana) service manuals (free PDFs on spicerparts.com), Yukon/Nitro install guides | ~20 MB |
| Body Builder (BBAS) 2016 Super Duty layout book (upfitter wiring, dimensions) | fleet.ford.com BBAS (free, public) | ~50 MB |
| 2016 RV & Trailer Towing Guide | Ford fleet/owner site (free) | ~5 MB |
| Your truck's own records | Window sticker by VIN, service history, OASIS printout, as-built data (FORScan export) | small, high value |

## Verification policy for the agent
- [OM] and [TSB] data can be stated as fact (still subject to VIN/build-date applicability).
- [FIELD] is guidance. [VERIFY] torque on safety-critical fasteners must be checked against the WSM before final torque.
