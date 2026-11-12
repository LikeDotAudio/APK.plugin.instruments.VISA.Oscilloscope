# SDK — INSTRUMENT.Oscilloscope

Every Oscilloscope model this library drives, and how to drive it. Each model answers the same five verbs over HTTP (its own port), WebSocket, a Unix socket and the bus; one page per model below lists its routes and every command.

← [Manual and Artifacts](INDEX.md)

| Verb | What it does |
|---|---|
| `get` | reads one value |
| `set` | writes one value |
| `nab` | reads more than one thing (observation, telemetry) |
| `rig` | configures several arguments at once |
| `do` | executes an action; takes no value |

| Model | Maker | get | set | nab | rig | do | Port |
|---|---|---:|---:|---:|---:|---:|---:|
| [54622D](SDK/54622D.md) | HP / Agilent / Keysight | 157 | 174 | 171 | 1 | 106 | 15200 |
| [54641D](SDK/54641D.md) | HP / Agilent / Keysight | 157 | 174 | 177 | 1 | 106 | 15201 |
| [DHO804](SDK/DHO804.md) | Rigol | 157 | 174 | 171 | 1 | 106 | 15202 |
| [DS1054Z](SDK/DS1054Z.md) | Rigol | 157 | 174 | 171 | 1 | 106 | 15203 |
| [DS1074Z](SDK/DS1074Z.md) | Rigol | 157 | 174 | 171 | 1 | 106 | 15204 |
| [DS1104Z](SDK/DS1104Z.md) | Rigol | 354 | 341 | 373 | 0 | 62 | 15205 |
| [DS1104Z Plus](SDK/DS1104Z%20Plus.md) | Rigol | 157 | 174 | 171 | 1 | 106 | 15206 |
| [DS7014](SDK/DS7014.md) | Rigol | 157 | 174 | 171 | 1 | 106 | 15207 |
| [DSO9064A](SDK/DSO9064A.md) | HP / Agilent / Keysight | 157 | 174 | 171 | 1 | 106 | 15208 |
| [DSO9104A](SDK/DSO9104A.md) | HP / Agilent / Keysight | 157 | 174 | 171 | 1 | 106 | 15209 |
| [DSOS054A](SDK/DSOS054A.md) | HP / Agilent / Keysight | 157 | 174 | 171 | 1 | 106 | 15210 |
| [DSOS104A](SDK/DSOS104A.md) | HP / Agilent / Keysight | 157 | 174 | 171 | 1 | 106 | 15211 |
| [DSOX1102G](SDK/DSOX1102G.md) | HP / Agilent / Keysight | 157 | 174 | 171 | 1 | 106 | 15212 |
| [DSOX2002A](SDK/DSOX2002A.md) | HP / Agilent / Keysight | 157 | 174 | 171 | 1 | 106 | 15213 |
| [DSOX4024A](SDK/DSOX4024A.md) | HP / Agilent / Keysight | 157 | 174 | 171 | 1 | 106 | 15214 |
| [HMO1002](SDK/HMO1002.md) | Rohde & Schwarz | 157 | 174 | 171 | 1 | 106 | 15215 |
| [MDO3014](SDK/MDO3014.md) | Tektronix | 157 | 174 | 171 | 1 | 106 | 15216 |
| [MDO4000C](SDK/MDO4000C.md) | Tektronix | 157 | 174 | 171 | 1 | 106 | 15217 |
| [MSO24](SDK/MSO24.md) | Tektronix | 157 | 174 | 171 | 1 | 106 | 15218 |
| [MSO44](SDK/MSO44.md) | Tektronix | 157 | 174 | 171 | 1 | 106 | 15219 |
| [MSO5074](SDK/MSO5074.md) | Rigol | 157 | 174 | 171 | 1 | 106 | 15220 |
| [MSO54](SDK/MSO54.md) | Tektronix | 157 | 174 | 171 | 1 | 106 | 15221 |
| [MSO64](SDK/MSO64.md) | Tektronix | 157 | 174 | 171 | 1 | 106 | 15222 |
| [MSOX3014T](SDK/MSOX3014T.md) | HP / Agilent / Keysight | 157 | 174 | 171 | 1 | 106 | 15223 |
| [MXO4](SDK/MXO4.md) | Rohde & Schwarz | 157 | 174 | 171 | 1 | 106 | 15224 |
| [RTB2002](SDK/RTB2002.md) | Rohde & Schwarz | 157 | 174 | 171 | 1 | 106 | 15225 |
| [RTB2004](SDK/RTB2004.md) | Rohde & Schwarz | 157 | 174 | 171 | 1 | 106 | 15226 |
| [RTH1002](SDK/RTH1002.md) | Rohde & Schwarz | 157 | 174 | 171 | 1 | 106 | 15227 |
| [RTM3004](SDK/RTM3004.md) | Rohde & Schwarz | 157 | 174 | 171 | 1 | 106 | 15228 |
| [TBS1052B](SDK/TBS1052B.md) | Tektronix | 157 | 174 | 171 | 1 | 106 | 15229 |
| [TBS2000B](SDK/TBS2000B.md) | Tektronix | 157 | 174 | 171 | 1 | 106 | 15230 |
| [TDS2024C](SDK/TDS2024C.md) | Tektronix | 157 | 174 | 171 | 1 | 106 | 15231 |
| [Z204](SDK/Z204.md) | HP / Agilent / Keysight | 157 | 174 | 171 | 1 | 106 | 15232 |
