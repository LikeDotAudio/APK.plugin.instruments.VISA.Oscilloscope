# Sources — 54641D.komand

Every change to this table that a vendor manual confirms, with where the manual says it (AUDIO.komand `check-tables --strict` research, 2026-10-31). A finding no manual confirmed is listed under *Not confirmed* with what was searched, and the table is left as it was.

## SCPI short form of the table's own long form (54641D)

SCPI-99 Vol 1 §6.2.1 abbreviation rule; the keyword as written in the Agilent InfiniiVision 6000 Series Programmer's Guide, :MARKer:X1Position, pp. 309-310 — <https://www.cfd.rit.edu/products/manuals/Agilent/oscilloscopes/6000_series_prog_guide.pdf>

| Command | Change | Manual |
|---|---|---|
| `set/Set_X1` | scpiFast = `"MARK:X1P <pos>"` | MARKer:X1Position — the short form is the capitals, X1P |
| `set/Set_X2` | scpiFast = `"MARK:X2P <pos>"` | MARKer:X2Position — the short form is the capitals, X2P |
| `set/Set_Y1` | scpiFast = `"MARK:Y1P <lev>"` | MARKer:Y1Position — the short form is the capitals, Y1P |
| `set/Set_Y2` | scpiFast = `"MARK:Y2P <lev>"` | MARKer:Y2Position — the short form is the capitals, Y2P |

### Not confirmed (left as is)

- `set/Set_Acquire_Mode` — searched: the 54641D's own manual — Keysight "54620/40-series Oscilloscopes Programmer's Guide" (asset 9018-40679) and the "54620/40-series Programmer's Reference" help file (9018-18242) — is served only behind Keysight's download form, which refused automated fetches; no mirror (xdevs.com, manualmachine, manualslib, archive.org) carries it. The successor Agilent InfiniiVision 6000 Series Programmer's Guide (2005-2010, https://www.cfd.rit.edu/products/manuals/Agilent/oscilloscopes/6000_series_prog_guide.pdf, pp. 43-46 "Command Differences From 54620/54640") documents the same node, but its value lists carry 6000-only options (SBUS, BUS, EITHer/ALTernate, SEGMented, I2S…), so it does not confirm the 54641D's set
- `set/Set_Acquire_Mode_AVERage` — searched: as above (54641D manual not obtainable)
- `set/Set_Acquire_Mode_HRESolution` — searched: as above (54641D manual not obtainable)
- `set/Set_Acquire_Mode_NORMal` — searched: as above (54641D manual not obtainable)
- `set/Set_Acquire_Mode_PEAK` — searched: as above (54641D manual not obtainable)
- `set/Set_Acquire_Type` — searched: as above (54641D manual not obtainable)
- `set/CH1_Coupling` — searched: as above (54641D manual not obtainable)
- `set/Set_Channel_Coupling` — searched: as above (54641D manual not obtainable)
- `set/CH2_Coupling` — searched: as above (54641D manual not obtainable)
- `set/Set_Coupling` — searched: as above (54641D manual not obtainable)
- `set/Set_Impedance` — searched: as above (54641D manual not obtainable)
- `set/Set_Display_Source` — searched: as above (54641D manual not obtainable)
- `set/Set_External_Impedance` — searched: as above (54641D manual not obtainable)
- `set/Set_External_Units` — searched: as above (54641D manual not obtainable)
- `set/Set_Function_Operation` — searched: as above (54641D manual not obtainable)
- `set/Set_Operation` — searched: as above (54641D manual not obtainable)
- `set/Set_Function_Reference` — searched: as above (54641D manual not obtainable)
- `set/Set_Source1` — searched: as above (54641D manual not obtainable)
- `set/Set_Source2` — searched: as above (54641D manual not obtainable)
- `set/Set_Window_FLATtop` — searched: as above (54641D manual not obtainable)
- `set/Set_Window_HANNing` — searched: as above (54641D manual not obtainable)
- `set/Set_Window_RECTangular` — searched: as above (54641D manual not obtainable)
- `set/Set_Hardcopy_Format` — searched: as above (54641D manual not obtainable)
- `set/Set_Marker_Mode` — searched: as above (54641D manual not obtainable)
- `set/Set_Measure_Source` — searched: as above (54641D manual not obtainable)
- `set/Set_Mode` — searched: as above (54641D manual not obtainable)
- `set/Set_Reference` — searched: as above (54641D manual not obtainable)
- `set/Set_Trigger_Can_Pattern_Id_Mode` — searched: as above (54641D manual not obtainable)
- `set/Set_Trigger_Can_Source` — searched: as above (54641D manual not obtainable)
- `set/Set_Edge_Slope` — searched: as above (54641D manual not obtainable)
- `set/Set_Edge_Source` — searched: as above (54641D manual not obtainable)
- `set/Set_Edge_Source_CH1` — searched: as above (54641D manual not obtainable)
- `set/Set_Edge_Source_CH2` — searched: as above (54641D manual not obtainable)
- `set/Set_Edge_Source_EXT` — searched: as above (54641D manual not obtainable)
- `set/Set_Trigger_Glitch_Polarity` — searched: as above (54641D manual not obtainable)
- `set/Set_Glitch_Source` — searched: as above (54641D manual not obtainable)
- `set/Set_Trigger_Lin_Source` — searched: as above (54641D manual not obtainable)
- `set/Set_Trigger_Mode` — searched: as above (54641D manual not obtainable)
- `set/Set_Trigger_Spi_Clock_Slope` — searched: as above (54641D manual not obtainable)
- `set/Set_Trigger_Sweep` — searched: as above (54641D manual not obtainable)
- `set/Set_Trigger_Tv_Mode` — searched: as above (54641D manual not obtainable)
- `set/Set_Trigger_Tv_Polarity` — searched: as above (54641D manual not obtainable)
- `set/Set_Trigger_Tv_Source` — searched: as above (54641D manual not obtainable)
- `set/Set_Waveform_Format` — searched: as above (54641D manual not obtainable)
- `set/Set_Waveform_Source` — searched: as above (54641D manual not obtainable)
- `rig/Setup_Trigger_Edge` — searched: as above (54641D manual not obtainable)

## SCPI paths — every header against the model's own tree (scpi_paths.py, 2026-11-11)

The tree: `54641D.scpi.json`, read off Agilent 54620/54640 Series Programmer's Guide; the 6000 Series Programmer's Guide (SOURCES.md) for the shared InfiniiVision tree. Each entry's `notes` / `retired_because` carries the full reason and page; the 33220A's Certify of 2026-11-11 (199 tries) and the GUI-certificate book are the bench evidence. Nothing was sent to verify.

| Command | Change | Was |
|---|---|---|
| `do/Do_Measure_Risetime` | scpi → `:MEASure:RISetime` | was `:MEASure:RISEtime` |
| `nab/Get_Marker_Xdelta` | scpi → `:MARKer:XDELta?` | was `:MARker:XDELta?` |
| `set/Set_Probe_Skew` | scpi → `:CHANnel<n>:PROBe:SKEW <value>` | was `:PROBe:SKEW <value>` |
| `nab/Get_Probe_Skew` | scpi → `:CHANnel<n>:PROBe:SKEW?` | was `PROBe:SKEW?` |
| `do/Do_Display_Line` | scpi → `:DISPlay:LINE` | was `DISPLay:LINE` |
| `do/Do_Protection_Clear` | left as is, unverified — unresolved |  |

## Options for the selectors (2026-11-11, owner: "if there are options, make it a selector AND individuals")

Agilent InfiniiVision 6000 Series Programmer's Guide (https://www.cfd.rit.edu/products/manuals/Agilent/oscilloscopes/6000_series_prog_guide.pdf). The 54641D's own guide is still not obtainable; the 6000's version-1.00 set is the 54620/40 set less the differences on pp. 43-46, and its version log (pp. 21-42) names every option added since. Each list below is the 6000 list less those additions; every individual SET is unverified until the bench sends it.

| Selector(s) | Options | Page — and what was left out |
|---|---|---|
| `Set_Acquire_Mode` | RTIMe ETIMe | p. 199 — SEGMented (v5.10) |
| `Set_Acquire_Type` | NORMal AVERage PEAK | p. 208 — HRESolution (v3.00, p. 41) |
| `CH1_Coupling` `CH2_Coupling` `Set_Channel_Coupling` `Set_Coupling` | AC DC | p. 233 |
| `Set_Impedance`, `Set_External_Impedance` | ONEMeg FIFTy | :CHANnel<n>:IMPedance / :EXTernal:IMPedance |
| `Set_Display_Source` | PMEMory0-2 | p. 264; p. 44: three pixel memories on the 5462x/4x |
| `Set_External_Units` | VOLT AMPere | :EXTernal:UNITs |
| `Set_Function_Operation` `Set_Operation` | SUBTract MULTiply INTegrate DIFFerentiate FFT SQRT | p. 285 — ADD (v5.15) |
| `Set_Marker_Mode` | OFF MEASurement MANual | p. 309 — WAVeform (v5.20) |
| `Set_Measure_Source` | CHANnel1-2 FUNCtion EXTernal DIGital0-15 | :MEASure:SOURce (MSO) |
| `Set_Mode` / `Set_Reference` | MAIN WINDow XY ROLL / LEFT CENTer RIGHt | :TIMebase:MODE / :TIMebase:REFerence |
| `Set_Trigger_Can_Pattern_Id_Mode` | STANdard EXTended | |
| `Set_Trigger_Can_Source` `Set_Glitch_Source` `Set_Trigger_Lin_Source` | CHANnel1-2 DIGital0-15 | MSO lists |
| `Set_Edge_Slope` | POSitive NEGative | p. 515 — EITHer/ALTernate left out (not shown on the 5462x/4x) |
| `Set_Edge_Source` | CHANnel1-2 DIGital0-15 EXTernal LINE | |
| `Set_Trigger_Glitch_Polarity` `Set_Trigger_Spi_Clock_Slope` `Set_Trigger_Tv_Polarity` | POSitive NEGative | |
| `Set_Trigger_Mode` | EDGE GLITch PATTern CAN DURation IIC LIN SEQuence SPI TV USB | p. 485 — EBURst (v3.00), FLEXray (v4.10), UART (v5.00), I2S (v5.25), M1553 (v6.00) |
| `Set_Trigger_Sweep` | AUTO NORMal | |
| `Set_Trigger_Tv_Mode` | F1 F2 ALLFields ALLLines LINE VERTical LINEF1 LINEF2 LINEAlt LINEVert | p. 604 — the 5462x/4x names (p. 45 "renamed; old forms still accepted") |
| `Set_Trigger_Tv_Source` | CHANnel1-2 | |
| `Set_Waveform_Format` | WORD BYTE ASCii | :WAVeform:FORMat |
| `Set_Waveform_Source` | CHANnel1-2 POD1-2 FUNCtion | p. 650 — SBUS (v3.00), BUS1/2 (v4.00) |

Also: `Set_Function_Reference` is a level (p. 287, NR3), now `numeric` V. `Set_Acquire_Mode_AVERage/NORMal/PEAK`, `Set_Window_FLATtop/HANNing/RECTangular` and `Set_Edge_Source_CH1/CH2/EXT` still carried their `<placeholder>` (a press was refused as unfilled) — the option each name carries is written in. `Set_Acquire_Mode_HRESolution` retired (HRESolution came with the 6000's v3.00).

Left without options: `Set_Source1` / `Set_Source2` — :FUNCtion:SOURce1/2 are 6000 v5.15 commands (p. 34); the 5462x/4x used :FUNCtion:SOURce. `Set_Hardcopy_Format` — p. 44 says the 5462x/4x list differed (TIFF, LASerjet, DESKjet, EPSon, SEIKo) but never gives it whole.
