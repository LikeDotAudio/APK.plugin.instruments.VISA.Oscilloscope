# Sources — DS1104Z.komand

Every change to this table that a vendor manual confirms, with where the manual says it (AUDIO.komand `check-tables --strict` research, 2026-10-31). A finding no manual confirmed is listed under *Not confirmed* with what was searched, and the table is left as it was.

## RIGOL MSO1000Z/DS1000Z Series Digital Oscilloscope Programming Guide

Dec. 2015 — <https://www.batronix.com/files/Rigol/Oszilloskope/_DS&MSO1000Z/MSO_DS1000Z_ProgrammingGuide_EN.pdf>

| Command | Change | Manual |
|---|---|---|
| `set/Set_Config_Format` | arg = `{"kind": "bool", "values": ["OFF", "ON"]}` | :DECoder<n>:CONFig:FORMat, p. 2-42 — <bool> {{1|ON}|{0|OFF}} — a switch, not an enum |
| `set/Set_Mod_Type` | arg = `{"kind": "enum", "values": ["AM", "FM"], "default": "AM"}` | [:SOURce[<n>]]:MOD:TYPe, p. 2-136 — <type> {AM|FM} |
| `set/Set_Output_Impedance` | arg = `{"kind": "enum", "values": ["OMEG", "FIFT"], "default": "OMEG"}` | [:SOURce[<n>]]:OUTPut[<n>]:IMPedance, p. 2-131 — <impedance> {OMEG|FIFTy} (OMEG = high-Z, FIFTy = 50 Ω) |
| `set/Set_Parallel_Polarity` | arg = `{"kind": "enum", "values": ["NEG", "POS"], "default": "POS"}`; description = `"Set or query the data polarity of parallel decoding"` | :DECoder<n>:PARallel:POLarity, p. 2-59 — <pol> {NEGative|POSitive} |
| `set/Set_Parallel_Source` | arg = `{"kind": "enum", "values": ["D0", "D1", "D2", "D3", "D4", "D5", "D6", "D7", "D8", "D9", "D10", "D11", "D12", "D13", "D14", "D15", "CHAN1", "CHAN2", "CHAN3", "CHAN4"]}`; description = `"Set or query the channel source of the data bit currently selected (parallel decoding)"` | :DECoder<n>:PARallel:SOURce, p. 2-58 — <src> {D0…D15|CHANnel1…CHANnel4} |
| `set/Set_Spi_Mode` | arg = `{"kind": "enum", "values": ["CS", "TIM"], "default": "TIM"}`; description = `"Set or query the frame synchronization mode of SPI decoding"` | :DECoder<n>:SPI:MODE, p. 2-53 — <CsTmo> {CS|TIMeout} |
| `set/Set_Spi_Polarity` | arg = `{"kind": "enum", "values": ["NEG", "POS"], "default": "POS"}`; description = `"Set or query the polarity of the SDA data line in SPI decoding"` | :DECoder<n>:SPI:POLarity, p. 2-54 — <pol> {NEGative|POSitive} |
| `set/Set_Spi_Select` | arg = `{"kind": "enum", "values": ["NCS", "CS"], "default": "NCS"}`; description = `"Set or query the CS polarity in SPI decoding"` | :DECoder<n>:SPI:SELect, p. 2-52 — <CsNcs> {NCS|CS} |
| `set/Set_Threshold_Channel` | arg = `{"kind": "numeric", "unit": "V"}` | :DECoder<n>:THREshold:CHANnel1…4, p. 2-40 — <thre> is Real, (-4 × VerticalScale − VerticalOffset) to (4 × VerticalScale − VerticalOffset) — a level, not an enum |
| `set/Set_Trigger_Delay_Type` | arg = `{"kind": "enum", "values": ["GRE", "LESS", "GLES", "GOUT"], "default": "GRE"}`; description = `"Set or query the delay type in delay trigger"` | :TRIGger:DELay:TYPe, p. 2-194 — <type> {GREater|LESS|GLESs|GOUT} |
| `set/Set_Uart_Polarity` | arg = `{"kind": "enum", "values": ["NEG", "POS"], "default": "POS"}`; description = `"Set or query the polarity of RS232 decoding"` | :DECoder<n>:UART:POLarity, p. 2-45 — <pol> {NEGative|POSitive} |

### Short forms (no table change)

`:TRIGger:DURATion…`, `:SYSTem:OPTion:UNINSTall`, `:CURSor:MANual:IXDELta?` — their `scpiFast` (`DURAT`, `UNINST`, `IXDEL`) is right: "If abbreviation is used, all the capital letters in the command must be written completely" (p. 1-6, *Command Abbreviation*). The checker now reads the short form off the long form's capitals instead of truncating to four letters (AUDIO.komand `fast_is_short_form`). `:TRIGger:DELay:SLOPA` / `SLOPB` are two nodes (p. 2-192 ff.), no longer reported as an alias.

## SCPI paths — every header against the model's own tree (scpi_paths.py, 2026-11-11)

The tree: `DS1104Z.scpi.json`, read off Rigol MSO1000Z/DS1000Z Programming Guide (2015), Chapter 2 Command System; [:SOURce[<n>]] is the default node of the source commands. Each entry's `notes` / `retired_because` carries the full reason and page; the 33220A's Certify of 2026-11-11 (199 tries) and the GUI-certificate book are the bench evidence. Nothing was sent to verify.

| Command | Change | Was |
|---|---|---|
| `set/Set_Config_Endian` | scpi → `:DECoder<n>:CONFig:ENDian <value>` | was `:CONFig:ENDian <value>` |
| `set/Set_Config_Format` | scpi → `:DECoder<n>:CONFig:FORMat <value>` | was `:CONFig:FORMat <value>` |
| `set/Set_Config_Label` | scpi → `:DECoder<n>:CONFig:LABel <value>` | was `:CONFig:LABel <value>` |
| `set/Set_Config_Line` | scpi → `:DECoder<n>:CONFig:LINE <value>` | was `:CONFig:LINE <value>` |
| `set/Set_Config_Width` | scpi → `:DECoder<n>:CONFig:WIDth <value>` | was `:CONFig:WIDth <value>` |
| `set/Set_Iic_Address` | scpi → `:DECoder<n>:IIC:ADDRess <value>` | was `:IIC:ADDRess <value>` |
| `set/Set_Iic_Clk` | scpi → `:DECoder<n>:IIC:CLK <value>` | was `:IIC:CLK <value>` |
| `set/Set_Iic_Data` | scpi → `:DECoder<n>:IIC:DATA <value>` | was `:IIC:DATA <value>` |
| `set/Set_Parallel_Bitx` | scpi → `:DECoder<n>:PARallel:BITX <value>` | was `:PARallel:BITX <value>` |
| `set/Set_Parallel_Ccompensation` | scpi → `:DECoder<n>:PARallel:CCOMpensation <value>` | was `:PARallel:CCOMpensation <value>` |
| `set/Set_Parallel_Clk` | scpi → `:DECoder<n>:PARallel:CLK <value>` | was `:PARallel:CLK <value>` |
| `set/Set_Parallel_Edge` | scpi → `:DECoder<n>:PARallel:EDGE <value>` | was `:PARallel:EDGE <value>` |
| `set/Set_Parallel_Nreject` | scpi → `:DECoder<n>:PARallel:NREJect <value>` | was `:PARallel:NREJect <value>` |
| `set/Set_Parallel_Nrtime` | scpi → `:DECoder<n>:PARallel:NRTime <value>` | was `:PARallel:NRTime <value>` |
| `set/Set_Parallel_Plot` | scpi → `:DECoder<n>:PARallel:PLOT <value>` | was `:PARallel:PLOT <value>` |
| `set/Set_Parallel_Polarity` | scpi → `:DECoder<n>:PARallel:POLarity <value>` | was `:PARallel:POLarity <value>` |
| `set/Set_Parallel_Source` | scpi → `:DECoder<n>:PARallel:SOURce <value>` | was `:PARallel:SOURce <value>` |
| `set/Set_Parallel_Width` | scpi → `:DECoder<n>:PARallel:WIDTh <value>` | was `:PARallel:WIDTh <value>` |
| `set/Set_Spi_Clk` | scpi → `:DECoder<n>:SPI:CLK <value>` | was `:SPI:CLK <value>` |
| `set/Set_Spi_Csrc` | scpi → `:DECoder<n>:SPI:CS <value>` | was `:SPI:CS <value>` |
| `set/Set_Spi_Edge` | scpi → `:DECoder<n>:SPI:EDGE <value>` | was `:SPI:EDGE <value>` |
| `set/Set_Spi_Endian` | scpi → `:DECoder<n>:SPI:ENDian <value>` | was `:SPI:ENDian <value>` |
| `set/Set_Spi_Miso` | scpi → `:DECoder<n>:SPI:MISO <value>` | was `:SPI:MISO <value>` |
| `set/Set_Spi_Mode` | scpi → `:DECoder<n>:SPI:MODE <value>` | was `:SPI:MODE <value>` |
| `set/Set_Spi_Mosi` | scpi → `:DECoder<n>:SPI:MOSI <value>` | was `:SPI:MOSI <value>` |
| `set/Set_Spi_Polarity` | scpi → `:DECoder<n>:SPI:POLarity <value>` | was `:SPI:POLarity <value>` |
| `set/Set_Spi_Select` | scpi → `:DECoder<n>:SPI:SELect <value>` | was `:SPI:SELect <value>` |
| `set/Set_Spi_Timebase` | scpi → `:DECoder<n>:SPI:TIMeout <value>` | was `:SPI:TIMeout <value>` |
| `set/Set_Spi_Width` | scpi → `:DECoder<n>:SPI:WIDTh <value>` | was `:SPI:WIDTh <value>` |
| `set/Set_Threshold_Channel` | scpi → `:DECoder<n>:THREshold:CHANnel<chan> <value>` | was `:THREshold:CHANnel<chan> <value>` |
| `set/Set_Uart_Baud` | scpi → `:DECoder<n>:UART:BAUD <value>` | was `:UART:BAUD <value>` |
| `set/Set_Uart_Endian` | scpi → `:DECoder<n>:UART:ENDian <value>` | was `:UART:ENDian <value>` |
| `set/Set_Uart_Parallel` | scpi → `:DECoder<n>:UART:PARity <value>` | was `:UART:PARity <value>` |
| `set/Set_Uart_Polarity` | scpi → `:DECoder<n>:UART:POLarity <value>` | was `:UART:POLarity <value>` |
| `set/Set_Uart_Rx` | scpi → `:DECoder<n>:UART:RX <value>` | was `:UART:RX <value>` |
| `set/Set_Uart_Stop` | scpi → `:DECoder<n>:UART:STOP <value>` | was `:UART:STOP <value>` |
| `set/Set_Uart_Tx` | scpi → `:DECoder<n>:UART:TX <value>` | was `:UART:TX <value>` |
| `set/Set_Uart_Width` | scpi → `:DECoder<n>:UART:WIDTh <value>` | was `:UART:WIDTh <value>` |
| `nab/Get_Config_Endian` | scpi → `:DECoder<n>:CONFig:ENDian?` | was `:CONFig:ENDian?` |
| `nab/Get_Config_Format` | scpi → `:DECoder<n>:CONFig:FORMat?` | was `:CONFig:FORMat?` |
| `nab/Get_Config_Label` | scpi → `:DECoder<n>:CONFig:LABel?` | was `:CONFig:LABel?` |
| `nab/Get_Config_Line` | scpi → `:DECoder<n>:CONFig:LINE?` | was `:CONFig:LINE?` |
| `nab/Get_Config_Srate` | scpi → `:DECoder<n>:CONFig:SRATe?` | was `:CONFig:SRATe?` |
| `nab/Get_Config_Width` | scpi → `:DECoder<n>:CONFig:WIDth?` | was `:CONFig:WIDth?` |
| `nab/Get_Iic_Address` | scpi → `:DECoder<n>:IIC:ADDRess?` | was `:IIC:ADDRess?` |
| `nab/Get_Iic_Clk` | scpi → `:DECoder<n>:IIC:CLK?` | was `:IIC:CLK?` |
| `nab/Get_Iic_Data` | scpi → `:DECoder<n>:IIC:DATA?` | was `:IIC:DATA?` |
| `nab/Get_Parallel_Bitx` | scpi → `:DECoder<n>:PARallel:BITX?` | was `:PARallel:BITX?` |
| `nab/Get_Parallel_Ccompensation` | scpi → `:DECoder<n>:PARallel:CCOMpensation?` | was `:PARallel:CCOMpensation?` |
| `nab/Get_Parallel_Clk` | scpi → `:DECoder<n>:PARallel:CLK?` | was `:PARallel:CLK?` |
| `nab/Get_Parallel_Edge` | scpi → `:DECoder<n>:PARallel:EDGE?` | was `:PARallel:EDGE?` |
| `nab/Get_Parallel_Nreject` | scpi → `:DECoder<n>:PARallel:NREJect?` | was `:PARallel:NREJect?` |
| `nab/Get_Parallel_Nrtime` | scpi → `:DECoder<n>:PARallel:NRTime?` | was `:PARallel:NRTime?` |
| `nab/Get_Parallel_Plot` | scpi → `:DECoder<n>:PARallel:PLOT?` | was `:PARallel:PLOT?` |
| `nab/Get_Parallel_Polarity` | scpi → `:DECoder<n>:PARallel:POLarity?` | was `:PARallel:POLarity?` |
| `nab/Get_Parallel_Source` | scpi → `:DECoder<n>:PARallel:SOURce?` | was `:PARallel:SOURce?` |
| `nab/Get_Parallel_Width` | scpi → `:DECoder<n>:PARallel:WIDTh?` | was `:PARallel:WIDTh?` |
| `nab/Get_Spi_Clk` | scpi → `:DECoder<n>:SPI:CLK?` | was `:SPI:CLK?` |
| `nab/Get_Spi_Csrc` | scpi → `:DECoder<n>:SPI:CS?` | was `:SPI:CS?` |
| `nab/Get_Spi_Edge` | scpi → `:DECoder<n>:SPI:EDGE?` | was `:SPI:EDGE?` |
| `nab/Get_Spi_Endian` | scpi → `:DECoder<n>:SPI:ENDian?` | was `:SPI:ENDian?` |
| `nab/Get_Spi_Miso` | scpi → `:DECoder<n>:SPI:MISO?` | was `:SPI:MISO?` |
| `nab/Get_Spi_Mode` | scpi → `:DECoder<n>:SPI:MODE?` | was `:SPI:MODE?` |
| `nab/Get_Spi_Mosi` | scpi → `:DECoder<n>:SPI:MOSI?` | was `:SPI:MOSI?` |
| `nab/Get_Spi_Polarity` | scpi → `:DECoder<n>:SPI:POLarity?` | was `:SPI:POLarity?` |
| `nab/Get_Spi_Select` | scpi → `:DECoder<n>:SPI:SELect?` | was `:SPI:SELect?` |
| `nab/Get_Spi_Timebase` | scpi → `:DECoder<n>:SPI:TIMeout?` | was `:SPI:TIMeout?` |
| `nab/Get_Spi_Width` | scpi → `:DECoder<n>:SPI:WIDTh?` | was `:SPI:WIDTh?` |
| `nab/Get_Threshold_Channel` | scpi → `:DECoder<n>:THREshold:CHANnel<chan>?` | was `:THREshold:CHANnel<chan>?` |
| `nab/Get_Uart_Baud` | scpi → `:DECoder<n>:UART:BAUD?` | was `:UART:BAUD?` |
| `nab/Get_Uart_Endian` | scpi → `:DECoder<n>:UART:ENDian?` | was `:UART:ENDian?` |
| `nab/Get_Uart_Parallel` | scpi → `:DECoder<n>:UART:PARity?` | was `:UART:PARity?` |
| `nab/Get_Uart_Polarity` | scpi → `:DECoder<n>:UART:POLarity?` | was `:UART:POLarity?` |
| `nab/Get_Uart_Rx` | scpi → `:DECoder<n>:UART:RX?` | was `:UART:RX?` |
| `nab/Get_Uart_Stop` | scpi → `:DECoder<n>:UART:STOP?` | was `:UART:STOP?` |
| `nab/Get_Uart_Tx` | scpi → `:DECoder<n>:UART:TX?` | was `:UART:TX?` |
| `nab/Get_Uart_Width` | scpi → `:DECoder<n>:UART:WIDTh?` | was `:UART:WIDTh?` |
| `set/Set_Immediate_Offset` | scpi → `:VOLTage:LEVel:IMMediate:OFFSet <value>` | was `:IMMediate:OFFSet <value>` |
| `nab/Get_Immediate_Offset` | scpi → `:VOLTage:LEVel:IMMediate:OFFSet?` | was `:IMMediate:OFFSet?` |
| `do/Auto` | scpi → `:AUToscale` | was `:AUTO` |
| `do/Do_Waveform_Sor` | retired — Retired: `:WAV:SOR` is not in the MSO1000Z/DS1000Z Programming Guide — SOR is no form of :WAVeform:SOURce (p. 2-217), which takes <source>; the scraper read it out of the "LabVIEW Programming Demo" listing. |  |
| `nab/Get_Stats_CH1` | scpi → `:MEASure:ITEM? VPP,CHANnel1;:MEASure:ITEM? VRMS,CHANnel1;:MEASure:ITEM? FREQuency,CHANnel1;:MEASure:ITEM? PDUTy,CHANnel1` | was `:MEASure:VPP? CHANnel1;:MEASure:VRMS? CHANnel1;:MEASure:FREQuency? CHANnel1;:MEASure:PDUTy? CHANnel1` |
| `nab/Get_Stats_CH2` | scpi → `:MEASure:ITEM? VPP,CHANnel2;:MEASure:ITEM? VRMS,CHANnel2;:MEASure:ITEM? FREQuency,CHANnel2;:MEASure:ITEM? PDUTy,CHANnel2` | was `:MEASure:VPP? CHANnel2;:MEASure:VRMS? CHANnel2;:MEASure:FREQuency? CHANnel2;:MEASure:PDUTy? CHANnel2` |
| `nab/Get_Stats_CH3` | scpi → `:MEASure:ITEM? VPP,CHANnel3;:MEASure:ITEM? VRMS,CHANnel3;:MEASure:ITEM? FREQuency,CHANnel3;:MEASure:ITEM? PDUTy,CHANnel3` | was `:MEASure:VPP? CHANnel3;:MEASure:VRMS? CHANnel3;:MEASure:FREQuency? CHANnel3;:MEASure:PDUTy? CHANnel3` |
| `nab/Get_Stats_CH4` | scpi → `:MEASure:ITEM? VPP,CHANnel4;:MEASure:ITEM? VRMS,CHANnel4;:MEASure:ITEM? FREQuency,CHANnel4;:MEASure:ITEM? PDUTy,CHANnel4` | was `:MEASure:VPP? CHANnel4;:MEASure:VRMS? CHANnel4;:MEASure:FREQuency? CHANnel4;:MEASure:PDUTy? CHANnel4` |
