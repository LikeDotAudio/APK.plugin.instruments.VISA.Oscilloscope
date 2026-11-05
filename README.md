# INSTRUMENT.Oscilloscope

**Wiki:** [Documentation/README.md](Documentation/README.md) — principles, architecture, delivery, and the [SDK](Documentation/%F0%9F%A7%A9Manual%20and%20Artifacts/SDK.md).

The **Oscilloscope** instruments of the APK.audio bench, as one thing: 33 models, their command tables and the family's panel. Oscilloscopes: waveforms on screen and measurements on them.

| | |
|---|---|
| **Is** | **inputs** — takes signals in — its connectors are inputs a patch can land on<br>**metering** — measures — its readings are numbers with units<br>**monitoring** — shows — a trace, a waveform or a display you watch |
| **Inputs** | each model's BIM part: /api/bim/parts?full=1&id=<part> — ports where side is "input" and domain is not "power" |
| **Recipe** | none — data, not a container: read in place by the stacks that bake `INSTRUMENTS` |
| **Source** | this repository (https://github.com/LikeDotAudio/APK.plugin.instruments.VISA.Oscilloscope.git), a submodule of [APK.plugin.instruments.VISA](https://github.com/LikeDotAudio/APK.plugin.instruments.VISA) at `INSTRUMENT.Oscilloscope/` |
| **Family name** | `Oscilloscope` — the device type, the topic segment and the `manifest.json` key; the `INSTRUMENT.` prefix belongs to the folder only |

## Models

| Model | Maker | What | Commands | Table | API |
|---|---|---|---:|:---:|---|
| [54622D](Documentation/%F0%9F%A7%A9Manual%20and%20Artifacts/SDK/54622D.md) | HP / Agilent / Keysight | Mixed Signal (2+16 Chan, 100MHz) | 452 |  | :15200 |
| [54641D](Documentation/%F0%9F%A7%A9Manual%20and%20Artifacts/SDK/54641D.md) | HP / Agilent / Keysight | Mixed Signal (2+16 Chan, 350MHz) | 452 | ✅ | :15201 |
| [DHO804](Documentation/%F0%9F%A7%A9Manual%20and%20Artifacts/SDK/DHO804.md) | Rigol | 70 MHz 4 Ch (12-bit High Res) | 452 |  | :15202 |
| [DS1054Z](Documentation/%F0%9F%A7%A9Manual%20and%20Artifacts/SDK/DS1054Z.md) | Rigol | 50 MHz 4 Ch (The 'Hobbyist Standard') | 452 |  | :15203 |
| [DS1074Z](Documentation/%F0%9F%A7%A9Manual%20and%20Artifacts/SDK/DS1074Z.md) | Rigol | 70 MHz 4 Ch | 452 |  | :15204 |
| [DS1104Z](Documentation/%F0%9F%A7%A9Manual%20and%20Artifacts/SDK/DS1104Z.md) | Rigol | 100 MHz 4 Ch Digital | 777 | ✅ | :15205 |
| [DS1104Z Plus](Documentation/%F0%9F%A7%A9Manual%20and%20Artifacts/SDK/DS1104Z%20Plus.md) | Rigol | 100 MHz 4 Ch (Upgradable) | 452 |  | :15206 |
| [DS7014](Documentation/%F0%9F%A7%A9Manual%20and%20Artifacts/SDK/DS7014.md) | Rigol | 100 MHz 4 Ch Performance | 452 |  | :15207 |
| [DSO9064A](Documentation/%F0%9F%A7%A9Manual%20and%20Artifacts/SDK/DSO9064A.md) | HP / Agilent / Keysight | 600 MHz 4 Ch (Infiniium 9000) | 452 |  | :15208 |
| [DSO9104A](Documentation/%F0%9F%A7%A9Manual%20and%20Artifacts/SDK/DSO9104A.md) | HP / Agilent / Keysight | 1 GHz 4 Ch (Infiniium 9000) | 452 |  | :15209 |
| [DSOS054A](Documentation/%F0%9F%A7%A9Manual%20and%20Artifacts/SDK/DSOS054A.md) | HP / Agilent / Keysight | 500 MHz 4 Ch (Infiniium S-Series) | 452 |  | :15210 |
| [DSOS104A](Documentation/%F0%9F%A7%A9Manual%20and%20Artifacts/SDK/DSOS104A.md) | HP / Agilent / Keysight | 1 GHz 4 Ch (Infiniium S-Series) | 452 |  | :15211 |
| [DSOX1102G](Documentation/%F0%9F%A7%A9Manual%20and%20Artifacts/SDK/DSOX1102G.md) | HP / Agilent / Keysight | 70/100 MHz 2 Ch + Gen (InfiniiVision 1000X) | 452 |  | :15212 |
| [DSOX2002A](Documentation/%F0%9F%A7%A9Manual%20and%20Artifacts/SDK/DSOX2002A.md) | HP / Agilent / Keysight | 70 MHz 2 Ch (InfiniiVision 2000X) | 452 |  | :15213 |
| [DSOX4024A](Documentation/%F0%9F%A7%A9Manual%20and%20Artifacts/SDK/DSOX4024A.md) | HP / Agilent / Keysight | 200 MHz 4 Ch (InfiniiVision 4000X) | 452 |  | :15214 |
| [HMO1002](Documentation/%F0%9F%A7%A9Manual%20and%20Artifacts/SDK/HMO1002.md) | Rohde & Schwarz | Mixed Signal 50-100MHz (Legacy Hameg) | 452 |  | :15215 |
| [MDO3014](Documentation/%F0%9F%A7%A9Manual%20and%20Artifacts/SDK/MDO3014.md) | Tektronix | Mixed Domain (Scope + Spectrum) | 452 |  | :15216 |
| [MDO4000C](Documentation/%F0%9F%A7%A9Manual%20and%20Artifacts/SDK/MDO4000C.md) | Tektronix | High Perf Mixed Domain | 452 |  | :15217 |
| [MSO24](Documentation/%F0%9F%A7%A9Manual%20and%20Artifacts/SDK/MSO24.md) | Tektronix | 2 Series Handheld/Bench (Battery) | 452 |  | :15218 |
| [MSO44](Documentation/%F0%9F%A7%A9Manual%20and%20Artifacts/SDK/MSO44.md) | Tektronix | 4 Series Mixed Signal | 452 |  | :15219 |
| [MSO5074](Documentation/%F0%9F%A7%A9Manual%20and%20Artifacts/SDK/MSO5074.md) | Rigol | 70 MHz 4 Ch Mixed Signal (Touch) | 452 |  | :15220 |
| [MSO54](Documentation/%F0%9F%A7%A9Manual%20and%20Artifacts/SDK/MSO54.md) | Tektronix | 5 Series Mixed Signal (8 FlexCh) | 452 |  | :15221 |
| [MSO64](Documentation/%F0%9F%A7%A9Manual%20and%20Artifacts/SDK/MSO64.md) | Tektronix | 6 Series Mixed Signal | 452 |  | :15222 |
| [MSOX3014T](Documentation/%F0%9F%A7%A9Manual%20and%20Artifacts/SDK/MSOX3014T.md) | HP / Agilent / Keysight | 100 MHz 4+16 Ch Touch (InfiniiVision 3000T) | 452 |  | :15223 |
| [MXO4](Documentation/%F0%9F%A7%A9Manual%20and%20Artifacts/SDK/MXO4.md) | Rohde & Schwarz | Next Gen High Speed Scope | 452 |  | :15224 |
| [RTB2002](Documentation/%F0%9F%A7%A9Manual%20and%20Artifacts/SDK/RTB2002.md) | Rohde & Schwarz | 70-300 MHz 2 Ch (10-bit ADC) | 452 |  | :15225 |
| [RTB2004](Documentation/%F0%9F%A7%A9Manual%20and%20Artifacts/SDK/RTB2004.md) | Rohde & Schwarz | 70-300 MHz 4 Ch (10-bit ADC) | 452 |  | :15226 |
| [RTH1002](Documentation/%F0%9F%A7%A9Manual%20and%20Artifacts/SDK/RTH1002.md) | Rohde & Schwarz | Scope Rider Handheld (Isolated) | 452 |  | :15227 |
| [RTM3004](Documentation/%F0%9F%A7%A9Manual%20and%20Artifacts/SDK/RTM3004.md) | Rohde & Schwarz | 100-1000 MHz 4 Ch (10-bit ADC) | 452 |  | :15228 |
| [TBS1052B](Documentation/%F0%9F%A7%A9Manual%20and%20Artifacts/SDK/TBS1052B.md) | Tektronix | 50 MHz 2 Ch (Basic) | 452 |  | :15229 |
| [TBS2000B](Documentation/%F0%9F%A7%A9Manual%20and%20Artifacts/SDK/TBS2000B.md) | Tektronix | Digital Storage Scope (Modern Basic) | 452 |  | :15230 |
| [TDS2024C](Documentation/%F0%9F%A7%A9Manual%20and%20Artifacts/SDK/TDS2024C.md) | Tektronix | 200 MHz 4 Ch (Legacy Workhorse) | 452 |  | :15231 |
| [Z204](Documentation/%F0%9F%A7%A9Manual%20and%20Artifacts/SDK/Z204.md) | HP / Agilent / Keysight | Generic Z-Series Reference | 452 |  | :15232 |

## Layout

```
INSTRUMENT.Oscilloscope/
  thing.json            what this thing is on the bench (authored)
  gui/                  the family panel, stamped once per discovered box
    Oscilloscope.cad.json
    Oscilloscope.dxf
    Oscilloscope.json
    Oscilloscope.probe.json
  <Model>/              <Model>.komand (the command table), <Model>.gui,
                        <Model>.api.json (generated), commands_tree.md, SOURCES.md
  Documentation/        the wiki; SDK/ is generated by _komand/family_sdk_docs.py
```

Generated by `_komand/family_sdk_docs.py` in the parent repository; edit `thing.json` or the
models, not this page.

<!-- wiki:smoke -->
**Smoke test** — ❌ FAIL 0/1 since 2026-11-04 20:50 EST — [results](Documentation/%F0%9F%A7%A9Manual%20and%20Artifacts/SMOKE.md)
<!-- /wiki:smoke -->
