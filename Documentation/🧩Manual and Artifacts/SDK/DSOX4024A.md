# DSOX4024A — Oscilloscope

← [SDK](../SDK.md)

**HP / Agilent / Keysight** — 200 MHz 4 Ch (InfiniiVision 4000X)

| | |
|---|---|
| Channels | 4 |
| HTTP | `:15214/api/instrument/Oscilloscope/DSOX4024A` |
| `spec` | `/api/instrument/Oscilloscope/DSOX4024A/DSOX4024A.api.json` |
| `health` | `/api/instrument/Oscilloscope/DSOX4024A/health` |
| `get` | `/api/instrument/Oscilloscope/DSOX4024A/get/<command>` |
| `set` | `/api/instrument/Oscilloscope/DSOX4024A/set/<command>` |
| `nab` | `/api/instrument/Oscilloscope/DSOX4024A/nab/<command>` |
| `rig` | `/api/instrument/Oscilloscope/DSOX4024A/rig/<command>` |
| `do` | `/api/instrument/Oscilloscope/DSOX4024A/do/<command>` |
| socket `ws` | `/ws/instrument/Oscilloscope/DSOX4024A` |
| socket `readings` | `/ws/instrument/Oscilloscope/DSOX4024A/readings` |
| socket `unix` | `/run/apk/instruments/Oscilloscope.DSOX4024A.sock` |

## `get` — reads one value (157)

| Command | SCPI | Argument | Group | |
|---|---|---|---|---|
| `Get_Ese` | `*ESE?` |  | Common | unverified |
| `Get_Esr` | `*ESR?` |  | Common | unverified |
| `Read_IDN` | `*IDN?` |  | Errors and ID |  |
| `Get_Lrn` | `*LRN?` |  | Common | unverified |
| `Get_Opc` | `*OPC?` |  | Common | unverified |
| `Get_Opt` | `*OPT?` |  | Common | unverified |
| `Get_Sre` | `*SRE?` |  | Common | unverified |
| `Get_Stb` | `*STB?` |  | Common | unverified |
| `Get_Tst` | `*TST?` |  | Common | unverified |
| `Get_Acquire_Complete` | `:ACQuire:COMPlete?` |  | ACQ | unverified |
| `Get_Acquire_Count` | `:ACQuire:COUNT?` |  | ACQ | unverified |
| `Get_Acquire_Mode` | `:ACQuire:MODE?` |  | ACQ | unverified |
| `Get_Acquire_Points` | `:ACQuire:POINts?` |  | ACQ | unverified |
| `Get_Sample_Rate` | `ACQuire:SRATe?` |  | Acquisition Readbacks |  |
| `Get_Calibrate_Date` | `:CALibrate:DATE?` |  | CAL | unverified |
| `Get_Calibrate_Label` | `:CALibrate:LABel?` |  | CAL | unverified |
| `Get_Calibrate_Switch` | `:CALibrate:SWITch?` |  | CAL | unverified |
| `Get_Calibrate_Time` | `:CALibrate:TIME?` |  | CAL | unverified |
| `Get_Channel_Coupling` | `:CHANNEL1:COUPLING?` |  | CHANNEL | unverified |
| `Get_Channel_Range` | `:CHANNEL1:RANGE?` |  | CHANNEL | unverified |
| `Get_Display_Data` | `:DISPlay:DATA?` |  | DISP | unverified |
| `Get_Display_Label` | `:DISPlay:LABel?` |  | DISP | unverified |
| `Get_Display_Persistence` | `:DISPlay:PERSistence?` |  | DISP | unverified |
| `Get_Display_Source` | `:DISPlay:SOURce?` |  | DISP | unverified |
| `Get_Display_Vectors` | `:DISPlay:VECTors?` |  | DISP | unverified |
| `Get_External_Bwlimit` | `:EXTernal:BWLimit?` |  | EXT | unverified |
| `Get_External_Impedance` | `:EXTernal:IMPedance?` |  | EXT | unverified |
| `Get_External_Probe` | `:EXTernal:PROBe?` |  | EXT | unverified |
| `Get_External_Protection` | `:EXTernal:PROTection?` |  | EXT | unverified |
| `Get_External_Range` | `:EXTernal:RANGe?` |  | EXT | unverified |
| `Get_External_Units` | `:EXTernal:UNITs?` |  | EXT | unverified |
| `Get_Function_Center` | `:FUNCtion:CENTer?` |  | FUNC | unverified |
| `Get_Function_Display` | `:FUNCtion:DISPlay?` |  | FUNC | unverified |
| `Get_Function_Offset` | `:FUNCtion:OFFSet?` |  | FUNC | unverified |
| `Get_Function_Operation` | `:FUNCtion:OPERation?` |  | FUNC | unverified |
| `Get_Function_Range` | `:FUNCtion:RANGe?` |  | FUNC | unverified |
| `Get_Function_Reference` | `:FUNCtion:REFerence?` |  | FUNC | unverified |
| `Get_Function_Source` | `:FUNCtion:SOURce?` |  | FUNC | unverified |
| `Get_Function_Span` | `:FUNCtion:SPAN?` |  | FUNC | unverified |
| `Get_Function_Window` | `:FUNCtion:WINDow?` |  | FUNC | unverified |
| `Get_Hardcopy_Factors` | `:HARDcopy:FACTors?` |  | HARD | unverified |
| `Get_Hardcopy_Ffeed` | `:HARDcopy:FFEed?` |  | HARD | unverified |
| `Get_Hardcopy_Format` | `:HARDcopy:FORMat?` |  | HARD | unverified |
| `Get_Hardcopy_Grayscale` | `:HARDcopy:GRAYscale?` |  | HARD | unverified |
| `Get_Marker_Mode` | `:MARKer:MODE?` |  | MARK | unverified |
| `Get_Marker_Xdelta` | `:MARker:XDELta?` |  | MAR | unverified |
| `Get_X_Delta` | `MARKer:XDELta?` |  | Cursor Deltas |  |
| `Get_Y_Delta` | `MARKer:YDELta?` |  | Cursor Deltas |  |
| `Get_Measure_Count` | `MEASure:COUNter?` |  | MEAS | unverified |
| `Get_Measure_Delay` | `:MEASure:DELay?` |  | MEAS | unverified |
| `Get_Measure_Falltime` | `:MEASure:FALLtime?` |  | MEAS | unverified |
| `Get_Measure_Nwidth` | `:MEASure:NWIDth?` |  | MEAS | unverified |
| `Get_Measure_Overshoot` | `:MEASure:OVERshoot?` |  | MEAS | unverified |
| `Get_Measure_Phase` | `:MEASure:PHASe?` |  | MEAS | unverified |
| `Get_Measure_Preshoot` | `:MEASure:PREShoot?` |  | MEAS | unverified |
| `Get_Measure_Pwidth` | `:MEASure:PWIDth?` |  | MEAS | unverified |
| `Get_Measure_Risetime` | `:MEASURE:RISETIME?` |  | MEASURE | unverified |
| `Get_Measure_Show` | `:MEASure:SHOW?` |  | MEAS | unverified |
| `Get_Measure_Source` | `:MEASure:SOURce?` |  | MEAS | unverified |
| `Get_Measure_Tedge` | `:MEASure:TEDGe?` |  | MEAS | unverified |
| `Get_Measure_Tvalue` | `:MEASure:TVALue?` |  | MEAS | unverified |
| `Get_Measure_Vamplitude` | `:MEASure:VAMPlitude?` |  | MEAS | unverified |
| `Get_Measure_Vbase` | `:MEASure:VBASe?` |  | MEAS | unverified |
| `Get_Measure_Vtime` | `:MEASure:VTIMe?` |  | MEAS | unverified |
| `Get_Measure_Vtop` | `:MEASure:VTOP?` |  | MEAS | unverified |
| `Get_Measure_Xmax` | `:MEASure:XMAX?` |  | MEAS | unverified |
| `Get_Measure_Xmin` | `:MEASure:XMIN?` |  | MEAS | unverified |
| `Get_Probe_Skew` | `PROBe:SKEW?` |  | PROB | unverified |
| `Get_System_Date` | `:SYSTem:DATE?` |  | SYST | unverified |
| `Get_Error` | `SYSTem:ERRor?` |  | System Utilities |  |
| `Read_Error` | `:SYSTem:ERRor?` |  | Errors and ID |  |
| `Get_System_Lock` | `:SYSTem:LOCK?` |  | SYST | unverified |
| `Get_Setup` | `SYSTem:SETup?` |  | System Utilities |  |
| `Get_System_Time` | `:SYSTem:TIME?` |  | SYST | unverified |
| `Get_Timebase_Mode` | `:TIMebase:MODE?` |  | TIM | unverified |
| `Get_Timebase_Position` | `:TIMebase:POSition?` |  | TIM | unverified |
| `Get_Timebase_Range` | `:TIMebase:RANGe?` |  | TIM | unverified |
| `Get_Timebase_Reference` | `:TIMebase:REFerence?` |  | TIM | unverified |
| `Get_Timebase_Scale` | `:TIMebase:SCALe?` |  | TIM | unverified |
| `Get_Timebase_Window_Position` | `:TIMebase:WINDow:POSition?` |  | TIM | unverified |
| `Get_Timebase_Window_Range` | `:TIMebase:WINDow:RANGe?` |  | TIM | unverified |
| `Get_Timebase_Window_Scale` | `:TIMebase:WINDow:SCALe?` |  | TIM | unverified |
| `Get_Trigger_Can_Acknowledge` | `:TRIGger:CAN:ACKNowledge?` |  | TRIG | unverified |
| `Get_Trigger_Can_Pattern_Data` | `:TRIGger:CAN:PATTern:DATA?` |  | TRIG | unverified |
| `Get_Trigger_Can_Pattern_Id_Mode` | `:TRIGger:CAN:PATTern:ID:MODE?` |  | TRIG | unverified |
| `Get_Trigger_Can_Pattern_Id` | `:TRIGger:CAN:PATTern:ID?` |  | TRIG | unverified |
| `Get_Trigger_Can_Samplepoint` | `:TRIGger:CAN:SAMPlepoint?` |  | TRIG | unverified |
| `Get_Trigger_Can_Signal_Baudrate` | `:TRIGger:CAN:SIGNal:BAUDrate?` |  | TRIG | unverified |
| `Get_Trigger_Can_Source` | `:TRIGger:CAN:SOURce?` |  | TRIG | unverified |
| `Get_Trigger_Can_Trigger` | `:TRIGger:CAN:TRIGer?` |  | TRIG | unverified |
| `Get_Trigger_Coupling` | `:TRIGger:COUPling?` |  | TRIG | unverified |
| `Get_Trigger_Duration_Greaterthan` | `:TRIGger:DURation:GREaterthan?` |  | TRIG | unverified |
| `Get_Trigger_Duration_Lessthan` | `:TRIGger:DURation:LESSthan?` |  | TRIG | unverified |
| `Get_Trigger_Duration_Pattern` | `:TRIGger:DURation:PATTern?` |  | TRIG | unverified |
| `Get_Trigger_Duration_Qualifier` | `:TRIGger:DURation:QUALifier?` |  | TRIG | unverified |
| `Get_Trigger_Duration_Range` | `:TRIGger:DURation:RANGe?` |  | TRIG | unverified |
| `Get_Trigger_Edge_Level` | `:TRIGger:EDGE:LEVel?` |  | TRIG | unverified |
| `Get_Trigger_Edge_Slope` | `:TRIGger:EDGE:SLOPe?` |  | TRIG | unverified |
| `Get_Trigger_Edge_Source` | `:TRIGger:EDGE:SOURce?` |  | TRIG | unverified |
| `Get_Trigger_Glitch_Greaterthan` | `:TRIGger:GLITch:GREaterthan?` |  | TRIG | unverified |
| `Get_Trigger_Glitch_Lessthan` | `:TRIGger:GLITch:LESSthan?` |  | TRIG | unverified |
| `Get_Trigger_Glitch_Level` | `:TRIGger:GLITch:LEVel?` |  | TRIG | unverified |
| `Get_Trigger_Glitch_Polarity` | `:TRIGger:GLITch:POLarity?` |  | TRIG | unverified |
| `Get_Trigger_Glitch_Qualifier` | `:TRIGger:GLITch:QUALifier?` |  | TRIG | unverified |
| `Get_Trigger_Glitch_Range` | `:TRIGger:GLITch:RANGe?` |  | TRIG | unverified |
| `Get_Trigger_Glitch_Source` | `:TRIGger:GLITch:SOURce?` |  | TRIG | unverified |
| `Get_Trigger_Hfreject` | `:TRIGger:HFReject?` |  | TRIG | unverified |
| `Get_Trigger_Holdoff` | `:TRIGger:HOLDoff?` |  | TRIG | unverified |
| `Get_Trigger_Iic_Pattern_Address` | `:TRIGger:IIC:PATTern:ADDRess?` |  | TRIG | unverified |
| `Get_Trigger_Iic_Pattern_Data` | `:TRIGger:IIC:PATTern:DATA?` |  | TRIG | unverified |
| `Get_Trigger_Iic_Trigger_Qualifier` | `:TRIGger:IIC:TRIGger:QUALifer?` |  | TRIG | unverified |
| `Get_Trigger_Lin_Signal_Baudrate` | `:TRIGger:LIN:SIGNal:BAUDrate?` |  | TRIG | unverified |
| `Get_Trigger_Lin_Source` | `:TRIGger:LIN:SOURce?` |  | TRIG | unverified |
| `Get_Trigger_Lin_Trigger` | `:TRIGger:LIN:TRIGger?` |  | TRIG | unverified |
| `Get_Trigger_Mode` | `:TRIGger:MODE?` |  | TRIG | unverified |
| `Get_Trigger_Nreject` | `:TRIGger:NREJect?` |  | TRIG | unverified |
| `Get_Trigger_Pattern` | `:TRIGger:PATTern?` |  | TRIG | unverified |
| `Get_Trigger_Reject` | `:TRIGger:REJect?` |  | TRIG | unverified |
| `Get_Trigger_Sequence_Count` | `:TRIGger:SEQuence:COUNt?` |  | TRIG | unverified |
| `Get_Trigger_Sequence_Find` | `:TRIGGER:SEQuence:FIND?` |  | TRIGGER | unverified |
| `Get_Trigger_Sequence_Reset` | `:TRIGGER:SEQuence:RESet?` |  | TRIGGER | unverified |
| `Get_Trigger_Sequence_Timebase` | `:TRIGGER:SEQuence:TIMer?` |  | TRIGGER | unverified |
| `Get_Trigger_Sequence_Trigger` | `:TRIGGER:SEQuence:TRIGger?` |  | TRIGGER | unverified |
| `Get_Trigger_Spi_Clock_Slope` | `:TRIGger:SPI:CLOCk:SLOPe?` |  | TRIG | unverified |
| `Get_Trigger_Spi_Clock_Timebase` | `:TRIGger:SPI:CLOCk:TIMeout?` |  | TRIG | unverified |
| `Get_Trigger_Spi_Frame` | `:TRIGger:SPI:FRAMing?` |  | TRIG | unverified |
| `Get_Trigger_Spi_Pattern_Data` | `:TRIGger:SPI:PATTern:DATA?` |  | TRIG | unverified |
| `Get_Trigger_Spi_Pattern_Width` | `:TRIGger:SPI:PATTern:WIDth?` |  | TRIG | unverified |
| `Get_Trigger_Spi_Source_Clock` | `:TRIGger:SPI:SOURce:CLOCk?` |  | TRIG | unverified |
| `Get_Trigger_Spi_Source_Data` | `:TRIGger:SPI:SOURce:DATA?` |  | TRIG | unverified |
| `Get_Trigger_Spi_Source_Frame` | `:TRIGger:SPI:SOURce:FRAMe?` |  | TRIG | unverified |
| `Get_Trigger_Sweep` | `:TRIGger:SWEep?` |  | TRIG | unverified |
| `Get_Trigger_Tv_Line` | `:TRIGger:TV:LINE?` |  | TRIG | unverified |
| `Get_Trigger_Tv_Mode` | `:TRIGger:TV:MODE?` |  | TRIG | unverified |
| `Get_Trigger_Tv_Polarity` | `:TRIGger:TV:POLarity?` |  | TRIG | unverified |
| `Get_Trigger_Tv_Source` | `:TRIGger:TV:SOURce?` |  | TRIG | unverified |
| `Get_Trigger_Tv_Standard` | `:TRIGger:TV:STANdard?` |  | TRIG | unverified |
| `Get_Trigger_Tv_Tvmode` | `:TRIGger:TV:TVMODE?` |  | TRIG | unverified |
| `Get_Trigger_Usb_Source_Dminus` | `:TRIGger:USB:SOURce:DMINus?` |  | TRIG | unverified |
| `Get_Trigger_Usb_Source_Dplus` | `:TRIGger:USB:SOURce:DPLus?` |  | TRIG | unverified |
| `Get_Trigger_Usb_Speed` | `:TRIGger:USB:SPEed?` |  | TRIG | unverified |
| `Get_Trigger_Usb_Trigger` | `:TRIGger:USB:TRIGger?` |  | TRIG | unverified |
| `Get_Waveform_Byteorder` | `:WAVeform:BYTeorder?` |  | WAV | unverified |
| `Get_Waveform_Count` | `:WAVeform:COUNt?` |  | WAV | unverified |
| `Get_Waveform_Data` | `WAVeform:DATA?` |  | Waveform Data Readbacks |  |
| `Get_Waveform_Format` | `:WAVeform:FORMat?` |  | WAV | unverified |
| `Get_Waveform_Points` | `:WAVeform:POINts?` |  | WAV | unverified |
| `Get_Preamble` | `WAVeform:PREamble?` |  | Waveform Data Readbacks |  |
| `Get_Waveform_Source` | `:WAVeform:SOURce?` |  | WAV | unverified |
| `Get_Waveform_Unsigned` | `:WAVeform:UNSigned?` |  | WAV | unverified |
| `Get_Waveform_View` | `:WAVeform:VIEW?` |  | WAV | unverified |
| `Get_Waveform_Xincrement` | `:WAVeform:XINCrement?` |  | WAV | unverified |
| `Get_Waveform_Xorigin` | `:WAVeform:XORigin?` |  | WAV | unverified |
| `Get_Waveform_Xreference` | `:WAVeform:XREFerence?` |  | WAV | unverified |
| `Get_Waveform_Yincrement` | `:WAVeform:YINCrement?` |  | WAV | unverified |
| `Get_Waveform_Yorigin` | `:WAVeform:YORigin?` |  | WAV | unverified |
| `Get_Waveform_Yreference` | `:WAVeform:YREFerence?` |  | WAV | unverified |

## `set` — writes one value (174)

| Command | SCPI | Argument | Group | |
|---|---|---|---|---|
| `Set_Ese` | `*ESE <value>` | integer | Common | unverified |
| `Set_Rcl` | `*RCL <value>` | integer | Common | unverified |
| `Set_Sav` | `*SAV <value>` | integer | Common | unverified |
| `Set_Sre` | `*SRE <value>` | integer | Common | unverified |
| `Set_Acquire_Complete` | `:ACQuire:COMPlete <value>` | unknown | ACQ | unverified |
| `Set_Average_Count` | `ACQuire:COUNt <count>` | integer | Acquisition Settings |  |
| `Set_Averaging_Count` | `:ACQuire:COUNt <count>` | integer | Acquire Mode & Averaging |  |
| `Set_Acquire_Mode` | `:ACQuire:MODE <value>` | enum | ACQ | unverified |
| `Set_Points` | `ACQuire:POINts <points>` | integer | Acquisition Settings |  |
| `Set_Acquire_Mode_AVERage` | `:ACQuire:TYPE <type>` | enum | Acquire Mode & Averaging |  |
| `Set_Acquire_Mode_HRESolution` | `:ACQuire:TYPE <type>` | enum | Acquire Mode & Averaging |  |
| `Set_Acquire_Mode_NORMal` | `:ACQuire:TYPE <type>` | enum | Acquire Mode & Averaging |  |
| `Set_Acquire_Mode_PEAK` | `:ACQuire:TYPE <type>` | enum | Acquire Mode & Averaging |  |
| `Set_Acquire_Type` | `ACQuire:TYPE <type>` | enum | Acquisition Settings |  |
| `Set_Calibrate_Label` | `:CALibrate:LABel <value>` | unknown | CAL | unverified |
| `CH1_BWLimit` | `:CHANnel1:BWLimit <state>` | OFF · ON | Vertical Setup CH1 |  |
| `CH1_Coupling` | `:CHANnel1:COUPling <coupling>` | enum | Vertical Setup CH1 |  |
| `Set_Channel_Coupling` | `:CHANNEL1:COUPLING <value>` | enum | CHANNEL | unverified |
| `CH1_Invert` | `:CHANnel1:INVert <state>` | OFF · ON | Vertical Setup CH1 |  |
| `CH1_Label` | `:CHANnel1:LABel <string>` | string | Vertical Setup CH1 |  |
| `CH1_Offset` | `:CHANnel1:OFFSet <offset>` | numeric | Vertical Setup CH1 |  |
| `CH1_Probe` | `:CHANnel1:PROBe <attenuation>` | numeric | Vertical Setup CH1 |  |
| `Set_Channel_Range` | `CHANnel1:RANGe <range>` | numeric | Channel 1 Settings |  |
| `CH1_Scale` | `:CHANnel1:SCALe <scale>` | numeric | Vertical Setup CH1 |  |
| `CH2_BWLimit` | `:CHANnel2:BWLimit <state>` | OFF · ON | Vertical Setup CH2 |  |
| `CH2_Coupling` | `:CHANnel2:COUPling <coupling>` | enum | Vertical Setup CH2 |  |
| `CH2_Invert` | `:CHANnel2:INVert <state>` | OFF · ON | Vertical Setup CH2 |  |
| `CH2_Label` | `:CHANnel2:LABel <string>` | string | Vertical Setup CH2 |  |
| `CH2_Offset` | `:CHANnel2:OFFSet <offset>` | numeric | Vertical Setup CH2 |  |
| `CH2_Probe` | `:CHANnel2:PROBe <attenuation>` | numeric | Vertical Setup CH2 |  |
| `CH2_Scale` | `:CHANnel2:SCALe <scale>` | numeric | Vertical Setup CH2 |  |
| `Set_Bandwidth_Limit` | `CHANnel<n>:BWLimit <state>` | OFF · ON | Analog Channel Settings |  |
| `Set_Coupling` | `CHANnel<n>:COUPling <coupling>` | enum | Analog Channel Settings |  |
| `Set_Display` | `CHANnel<n>:DISPlay <state>` | OFF · ON | Analog Channel Settings |  |
| `Set_Impedance` | `CHANnel<n>:IMPedance <imp>` | enum | Analog Channel Settings |  |
| `Set_Invert` | `CHANnel<n>:INVert <state>` | OFF · ON | Analog Channel Settings |  |
| `Set_Channel_Offset` | `:CHANnel<n>:OFFSet <offset>` | numeric | Analog Channel Settings | unverified |
| `Set_Probe` | `CHANnel<n>:PROBe <atten>` | numeric | Analog Channel Settings |  |
| `Set_Channel_Scale` | `:CHANnel<n>:SCALe <scale>` | numeric | Analog Channel Settings | unverified |
| `Set_Digital_Display` | `DIGital<n>:DISPlay <state>` | OFF · ON | Digital Channel (MSO) Settings |  |
| `Set_Digital_Label` | `DIGital<n>:LABel <label>` | unknown | Digital Channel (MSO) Settings |  |
| `Set_Digital_Position` | `DIGital<n>:POSition <pos>` | numeric | Digital Channel (MSO) Settings |  |
| `Set_Display_Data` | `:DISPlay:DATA <value>` | block | DISP | unverified |
| `Set_Display_Label` | `:DISPlay:LABel <value>` | unknown | DISP | unverified |
| `Set_Display_Persistence` | `DISPlay:PERSistence <value>` | numeric | DISP | unverified |
| `Set_Display_Source` | `:DISPlay:SOURce <value>` | enum | DISP | unverified |
| `Set_Display_Vectors` | `DISPlay:VECTors <value>` | unknown | DISP | unverified |
| `Set_External_Bwlimit` | `:EXTernal:BWLimit <value>` | OFF · ON | EXT | unverified |
| `Set_External_Impedance` | `EXTernal:IMPedance <value>` | enum | EXT | unverified |
| `Set_External_Probe` | `:EXTernal:PROBe <value>` | numeric | EXT | unverified |
| `Set_External_Range` | `:EXTernal:RANGe <value>` | numeric | EXT | unverified |
| `Set_External_Units` | `:EXTernal:UNITs <value>` | enum | EXT | unverified |
| `Set_Center_Frequency` | `:FUNCtion:CENTer <frequency>` | numeric | FFT Specific Configuration |  |
| `Set_Math_Display` | `:FUNCtion:DISPlay <state>` | OFF · ON | Math_FFT | unverified |
| `Set_Math_Offset` | `:FUNCtion:OFFSet <offset>` | numeric | Vertical Scale & Offset |  |
| `Set_Function_Operation` | `FUNCtion:OPERation <op>` | enum | Math Function Settings |  |
| `Set_Operation` | `:FUNCtion:OPERation <operation>` | enum | Select Operation |  |
| `Set_Math_Operator` | `:FUNCtion:OPERation <value>` | ADD · SUBT · MULT · DIFF · INT · FFT | Math_FFT | unverified |
| `Set_Math_Range` | `:FUNCtion:RANGe <range>` | numeric | Vertical Scale & Offset |  |
| `Set_Math_Scale` | `:FUNCtion:RANGe <value>` | numeric | Math_FFT | unverified |
| `Set_Function_Reference` | `:FUNCtion:REFerence <value>` | enum | FUNC | unverified |
| `Set_FFT_Scale` | `:FUNCtion:SCALe <scale>` | numeric | FFT Specific Configuration |  |
| `Set_Source1` | `FUNCtion:SOURce1 <src>` | enum | Math Function Settings |  |
| `Set_Source2` | `FUNCtion:SOURce2 <src>` | enum | Math Function Settings |  |
| `Set_Span` | `:FUNCtion:SPAN <span>` | numeric | FFT Specific Configuration |  |
| `Set_Window_FLATtop` | `:FUNCtion:WINDow <window>` | enum | FFT Specific Configuration |  |
| `Set_Window_HANNing` | `:FUNCtion:WINDow <window>` | enum | FFT Specific Configuration |  |
| `Set_Window_RECTangular` | `:FUNCtion:WINDow <window>` | enum | FFT Specific Configuration |  |
| `Set_Hardcopy_Factors` | `:HARDcopy:FACTors <value>` | unknown | HARD | unverified |
| `Set_Hardcopy_Ffeed` | `:HARDcopy:FFEed <value>` | unknown | HARD | unverified |
| `Set_Hardcopy_Format` | `HARDcopy:FORMat <value>` | enum | HARD | unverified |
| `Set_Hardcopy_Grayscale` | `:HARDcopy:GRAYscale <value>` | unknown | HARD | unverified |
| `Set_Marker_Mode` | `MARKer:MODE <mode>` | enum | Cursor Settings |  |
| `Set_X1` | `MARKer:X1Position <pos>` | numeric | Time/Frequency Markers |  |
| `Set_X2` | `MARKer:X2Position <pos>` | numeric | Time/Frequency Markers |  |
| `Set_Y1` | `MARKer:Y1Position <lev>` | numeric | Voltage Markers |  |
| `Set_Y2` | `MARKer:Y2Position <lev>` | numeric | Voltage Markers |  |
| `Set_Measure_Count` | `:MEASure:COUNter <value>` | integer | MEAS | unverified |
| `Set_Measure_Thresholds` | `MEASure:DEFine:THResholds <mode>` | numeric | Measurement Settings |  |
| `Set_Measure_Delay` | `:MEASure:DELay <value>` | numeric | MEAS | unverified |
| `Set_Measure_Falltime` | `:MEASure:FALLtime <value>` | numeric | MEAS | unverified |
| `Set_Measure_Nwidth` | `:MEASure:NWIDth <value>` | unknown | MEAS | unverified |
| `Set_Measure_Overshoot` | `:MEASure:OVERshoot <value>` | unknown | MEAS | unverified |
| `Set_Measure_Phase` | `:MEASure:PHASe <value>` | unknown | MEAS | unverified |
| `Set_Measure_Preshoot` | `:MEASure:PREShoot <value>` | block | MEAS | unverified |
| `Set_Measure_Pwidth` | `:MEASure:PWIDth <value>` | unknown | MEAS | unverified |
| `Set_Measure_Show` | `:MEASure:SHOW <value>` | unknown | MEAS | unverified |
| `Set_Measure_Source` | `MEASure:SOURce <source>` | enum | Measurement Settings |  |
| `Set_Measure_Tedge` | `:MEASure:TEDGe <value>` | unknown | MEAS | unverified |
| `Set_Measure_Tvalue` | `MEASure:TVALue <value>` | unknown | MEAS | unverified |
| `Set_Measure_Vamplitude` | `:MEASure:VAMPlitude <value>` | unknown | MEAS | unverified |
| `Set_Measure_Vbase` | `:MEASure:VBASe <value>` | unknown | MEAS | unverified |
| `Set_Measure_Vtop` | `:MEASure:VTOP <value>` | unknown | MEAS | unverified |
| `Set_Measure_Xmax` | `MEASure:XMAX <value>` | numeric | MEAS | unverified |
| `Set_Measure_Xmin` | `MEASure:XMIN <value>` | numeric | MEAS | unverified |
| `Set_Pod_Threshold` | `POD<n>:THReshold <thresh>` | numeric | Digital Channel (MSO) Settings |  |
| `Set_Probe_Skew` | `:PROBe:SKEW <value>` | numeric | PROB | unverified |
| `Set_System_Date` | `:SYSTem:DATE <value>` | unknown | SYST | unverified |
| `Set_System_Dsp` | `SYSTem:DSP <string>` | string | SYST | unverified |
| `Lock_Front_Panel` | `SYSTem:LOCK <state>` | OFF · ON | System Control |  |
| `Set_System_Time` | `:SYSTem:TIME <value>` | numeric | SYST | unverified |
| `Set_Mode` | `TIMebase:MODE <mode>` | enum | Timebase (Horizontal) Settings |  |
| `Set_Timebase_Delay` | `:TIMebase:POSition <delay>` | numeric | Horizontal Controls | unverified |
| `Set_Position` | `TIMebase:POSition <pos>` | numeric | Timebase (Horizontal) Settings |  |
| `Set_Timebase_Position` | `:TIMebase:POSition <position>` | numeric | Horizontal Controls |  |
| `Set_Timebase_Range` | `:TIMebase:RANGe <value>` | numeric | TIM | unverified |
| `Set_Reference` | `TIMebase:REFerence <ref>` | enum | Timebase (Horizontal) Settings |  |
| `Set_Timebase_Scale` | `:TIMebase:SCALe <scale>` | numeric | Horizontal Controls |  |
| `Set_Window_Position` | `TIMebase:WINDow:POSition <pos>` | numeric | Zoom Window Settings |  |
| `Set_Timebase_Window_Range` | `:TIMebase:WINDow:RANGe <value>` | numeric | TIM | unverified |
| `Set_Window_Scale` | `TIMebase:WINDow:SCALe <scale>` | numeric | Zoom Window Settings |  |
| `Set_Trigger_Can_Acknowledge` | `:TRIGger:CAN:ACKNowledge <value>` | unknown | TRIG | unverified |
| `Set_Trigger_Can_Pattern_Data` | `:TRIGger:CAN:PATTern:DATA <value>` | block | TRIG | unverified |
| `Set_Trigger_Can_Pattern_Id` | `TRIGger:CAN:PATTern:ID <value>` | unknown | TRIG | unverified |
| `Set_Trigger_Can_Pattern_Id_Mode` | `:TRIGger:CAN:PATTern:ID:MODE <value>` | enum | TRIG | unverified |
| `Set_Trigger_Can_Samplepoint` | `:TRIGger:CAN:SAMPlepoint <value>` | unknown | TRIG | unverified |
| `Set_Trigger_Can_Signal_Baudrate` | `:TRIGger:CAN:SIGNal:BAUDrate <value>` | unknown | TRIG | unverified |
| `Set_Trigger_Can_Source` | `:TRIGger:CAN:SOURce <value>` | enum | TRIG | unverified |
| `Set_Trigger_Can_Trigger` | `:TRIGger:CAN:TRIGger <value>` | unknown | TRIG | unverified |
| `Set_Trigger_Duration_Pattern` | `:TRIGger:DURation:PATTern <value>` | unknown | TRIG | unverified |
| `Set_Trigger_Duration_Qualifier` | `:TRIGger:DURation:QUALifier <value>` | unknown | TRIG | unverified |
| `Set_Trigger_Duration_Range` | `:TRIGger:DURation:RANGe <value>` | numeric | TRIG | unverified |
| `Set_Trigger_Level` | `:TRIGger:EDGE:LEVel <level>` | numeric | Trigger Configuration |  |
| `Set_Edge_Slope` | `TRIGger:EDGE:SLOPe <slope>` | enum | Edge Trigger Config |  |
| `Set_Edge_Source` | `TRIGger:EDGE:SOURce <source>` | enum | Edge Trigger Config |  |
| `Set_Edge_Source_CH1` | `:TRIGger:EDGE:SOURce <source>` | enum | Trigger Configuration |  |
| `Set_Edge_Source_CH2` | `:TRIGger:EDGE:SOURce <source>` | enum | Trigger Configuration |  |
| `Set_Edge_Source_EXT` | `:TRIGger:EDGE:SOURce <source>` | enum | Trigger Configuration |  |
| `Set_Glitch_Width` | `TRIGger:GLITch:LESSthan <time>` | numeric | Glitch/Pulse Width Config |  |
| `Set_Trigger_Glitch_Level` | `:TRIGger:GLITch:LEVel <value>` | numeric | TRIG | unverified |
| `Set_Trigger_Glitch_Polarity` | `:TRIGger:GLITch:POLarity <value>` | enum | TRIG | unverified |
| `Set_Glitch_Condition` | `TRIGger:GLITch:QUALifier <qual>` | unknown | Glitch/Pulse Width Config |  |
| `Set_Trigger_Glitch_Range` | `:TRIGger:GLITch:RANGe <value>` | numeric | TRIG | unverified |
| `Set_Glitch_Source` | `TRIGger:GLITch:SOURce <source>` | enum | Glitch/Pulse Width Config |  |
| `Set_Trigger_Hfreject` | `:TRIGger:HFReject <value>` | unknown | TRIG | unverified |
| `Set_Holdoff` | `TRIGger:HOLDoff <time>` | numeric | Trigger Settings |  |
| `Set_Trigger_Iic_Pattern_Address` | `:TRIGger:IIC:PATTern:ADDRess <value>` | integer | TRIG | unverified |
| `Set_Trigger_Iic_Pattern_Data` | `:TRIGger:IIC:PATTern:DATA <value>` | block | TRIG | unverified |
| `Set_Trigger_Iic_Trigger_Qualifier` | `:TRIGger:IIC:TRIGger:QUALifier <value>` | unknown | TRIG | unverified |
| `Set_Trigger_Lin_Signal_Baudrate` | `:TRIGger:LIN:SIGNal:BAUDrate <value>` | unknown | TRIG | unverified |
| `Set_Trigger_Lin_Source` | `:TRIGger:LIN:SOURce <value>` | enum | TRIG | unverified |
| `Set_Trigger_Lin_Trigger` | `:TRIGger:LIN:TRIGger <value>` | unknown | TRIG | unverified |
| `Set_Trigger_Mode` | `:TRIGger:MODE <mode>` | enum | Trigger Configuration |  |
| `Set_Trigger_Nreject` | `:TRIGger:NREJect <value>` | OFF · ON | TRIG | unverified |
| `Set_Trigger_Pattern` | `:TRIGger:PATTern <value>` | unknown | TRIG | unverified |
| `Set_Trigger_Sequence_Count` | `:TRIGger:SEQuence:COUNt <value>` | integer | TRIG | unverified |
| `Set_Trigger_Sequence_Find` | `:TRIGGER:SEQuence:FIND <value>` | unknown | TRIGGER | unverified |
| `Set_Trigger_Sequence_Reset` | `:TRIGGER:SEQuence:RESet <value>` | unknown | TRIGGER | unverified |
| `Set_Trigger_Sequence_Timebase` | `:TRIGGER:SEQuence:TIMer <value>` | numeric | TRIGGER | unverified |
| `Set_Trigger_Sequence_Trigger` | `:TRIGGER:SEQuence:TRIGger <value>` | unknown | TRIGGER | unverified |
| `Set_Trigger_Spi_Clock_Slope` | `:TRIGger:SPI:CLOCk:SLOPe <value>` | enum | TRIG | unverified |
| `Set_Trigger_Spi_Clock_Timebase` | `:TRIGger:SPI:CLOCk:TIMeout <value>` | numeric | TRIG | unverified |
| `Set_Trigger_Spi_Frame` | `:TRIGger:SPI:FRAMing <value>` | unknown | TRIG | unverified |
| `Set_Trigger_Spi_Pattern_Data` | `:TRIGger:SPI:PATTern:DATA <value>` | block | TRIG | unverified |
| `Set_Trigger_Spi_Pattern_Width` | `TRIGger:SPI:PATTern:WIDth <value>` | numeric | TRIG | unverified |
| `Set_Trigger_Spi_Source_Clock` | `:TRIGger:SPI:SOURce:CLOCk <value>` | unknown | TRIG | unverified |
| `Set_Trigger_Spi_Source_Data` | `:TRIGger:SPI:SOURce:DATA <value>` | block | TRIG | unverified |
| `Set_Trigger_Spi_Source_Frame` | `:TRIGger:SPI:SOURce:FRAMe <value>` | unknown | TRIG | unverified |
| `Set_Trigger_Sweep` | `:TRIGger:SWEep <sweep>` | enum | Trigger Configuration |  |
| `Set_Trigger_Tv_Line` | `:TRIGger:TV:LINE <value>` | unknown | TRIG | unverified |
| `Set_Trigger_Tv_Mode` | `TRIGger:TV:MODE <value>` | enum | TRIG | unverified |
| `Set_Trigger_Tv_Polarity` | `:TRIGger:TV:POLarity <value>` | enum | TRIG | unverified |
| `Set_Trigger_Tv_Source` | `:TRIGger:TV:SOURce <value>` | enum | TRIG | unverified |
| `Set_Trigger_Tv_Standard` | `:TRIGger:TV:STANdard <value>` | unknown | TRIG | unverified |
| `Set_Trigger_Usb_Source_Dminus` | `:TRIGger:USB:SOURce:DMINus <value>` | unknown | TRIG | unverified |
| `Set_Trigger_Usb_Source_Dplus` | `:TRIGger:USB:SOURce:DPLus <value>` | unknown | TRIG | unverified |
| `Set_Trigger_Usb_Speed` | `:TRIGger:USB:SPEed <value>` | numeric | TRIG | unverified |
| `Set_Trigger_Usb_Trigger` | `:TRIGger:USB:TRIGer <value>` | unknown | TRIG | unverified |
| `Set_Byte_Order` | `WAVeform:BYTeorder <order>` | unknown | Waveform Data Transfer Settings |  |
| `Set_Waveform_Format` | `WAVeform:FORMat <format>` | enum | Waveform Data Transfer Settings |  |
| `Set_Waveform_Points` | `WAVeform:POINts <points>` | integer | Waveform Data Transfer Settings |  |
| `Set_Waveform_Source` | `WAVeform:SOURce <source>` | enum | Waveform Data Transfer Settings |  |
| `Set_Unsigned` | `WAVeform:UNSigned <state>` | OFF · ON | Waveform Data Transfer Settings |  |
| `Set_Waveform_View` | `:WAVeform:VIEW <value>` | unknown | WAV | unverified |

## `nab` — reads more than one thing (observation, telemetry) (171)

| Command | SCPI | Argument | Group | |
|---|---|---|---|---|
| `Get_Ese` | `*ESE?` |  | Common | unverified |
| `Get_Esr` | `*ESR?` |  | Common | unverified |
| `Read_IDN` | `*IDN?` |  | Errors and ID |  |
| `Get_Lrn` | `*LRN?` |  | Common | unverified |
| `Get_Opc` | `*OPC?` |  | Common | unverified |
| `Get_Opt` | `*OPT?` |  | Common | unverified |
| `Get_Sre` | `*SRE?` |  | Common | unverified |
| `Get_Stb` | `*STB?` |  | Common | unverified |
| `Get_Tst` | `*TST?` |  | Common | unverified |
| `Get_Acquire_Complete` | `:ACQuire:COMPlete?` |  | ACQ | unverified |
| `Get_Acquire_Count` | `:ACQuire:COUNT?` |  | ACQ | unverified |
| `Get_Acquire_Mode` | `:ACQuire:MODE?` |  | ACQ | unverified |
| `Get_Acquire_Points` | `:ACQuire:POINts?` |  | ACQ | unverified |
| `Get_Sample_Rate` | `ACQuire:SRATe?` |  | Acquisition Readbacks |  |
| `Get_Calibrate_Date` | `:CALibrate:DATE?` |  | CAL | unverified |
| `Get_Calibrate_Label` | `:CALibrate:LABel?` |  | CAL | unverified |
| `Get_Calibrate_Switch` | `:CALibrate:SWITch?` |  | CAL | unverified |
| `Get_Calibrate_Time` | `:CALibrate:TIME?` |  | CAL | unverified |
| `Get_Channel_Coupling` | `:CHANNEL1:COUPLING?` |  | CHANNEL | unverified |
| `channel_settings_1` | `:CHANnel1:DISPlay?;:CHANnel1:SCALe?;:CHANnel1:OFFSet?` |  | CHANnel | unverified |
| `Get_Channel_Range` | `:CHANNEL1:RANGE?` |  | CHANNEL | unverified |
| `channel_settings_2` | `:CHANnel2:DISPlay?;:CHANnel2:SCALe?;:CHANnel2:OFFSet?` |  | CHANnel | unverified |
| `Get_Display_Data` | `:DISPlay:DATA?` |  | DISP | unverified |
| `Get_Display_Label` | `:DISPlay:LABel?` |  | DISP | unverified |
| `Get_Display_Persistence` | `:DISPlay:PERSistence?` |  | DISP | unverified |
| `Get_Display_Source` | `:DISPlay:SOURce?` |  | DISP | unverified |
| `Get_Display_Vectors` | `:DISPlay:VECTors?` |  | DISP | unverified |
| `Get_External_Bwlimit` | `:EXTernal:BWLimit?` |  | EXT | unverified |
| `Get_External_Impedance` | `:EXTernal:IMPedance?` |  | EXT | unverified |
| `Get_External_Probe` | `:EXTernal:PROBe?` |  | EXT | unverified |
| `Get_External_Protection` | `:EXTernal:PROTection?` |  | EXT | unverified |
| `Get_External_Range` | `:EXTernal:RANGe?` |  | EXT | unverified |
| `Get_External_Units` | `:EXTernal:UNITs?` |  | EXT | unverified |
| `Get_Function_Center` | `:FUNCtion:CENTer?` |  | FUNC | unverified |
| `Get_Function_Display` | `:FUNCtion:DISPlay?` |  | FUNC | unverified |
| `math_settings` | `:FUNCtion:DISPlay?;:FUNCtion:OPERation?;:FUNCtion:RANGe?;:FUNCtion:OFFSet?` |  | MATH | unverified |
| `Get_Function_Offset` | `:FUNCtion:OFFSet?` |  | FUNC | unverified |
| `Get_Function_Operation` | `:FUNCtion:OPERation?` |  | FUNC | unverified |
| `Get_Function_Range` | `:FUNCtion:RANGe?` |  | FUNC | unverified |
| `Get_Function_Reference` | `:FUNCtion:REFerence?` |  | FUNC | unverified |
| `Get_Function_Source` | `:FUNCtion:SOURce?` |  | FUNC | unverified |
| `Get_Function_Span` | `:FUNCtion:SPAN?` |  | FUNC | unverified |
| `Get_Function_Window` | `:FUNCtion:WINDow?` |  | FUNC | unverified |
| `Get_Hardcopy_Factors` | `:HARDcopy:FACTors?` |  | HARD | unverified |
| `Get_Hardcopy_Ffeed` | `:HARDcopy:FFEed?` |  | HARD | unverified |
| `Get_Hardcopy_Format` | `:HARDcopy:FORMat?` |  | HARD | unverified |
| `Get_Hardcopy_Grayscale` | `:HARDcopy:GRAYscale?` |  | HARD | unverified |
| `Get_Marker_Mode` | `:MARKer:MODE?` |  | MARK | unverified |
| `Get_Marker_Xdelta` | `:MARker:XDELta?` |  | MAR | unverified |
| `Get_X_Delta` | `MARKer:XDELta?` |  | Cursor Deltas |  |
| `Get_Y_Delta` | `MARKer:YDELta?` |  | Cursor Deltas |  |
| `Get_Measure_Count` | `MEASure:COUNter?` |  | MEAS | unverified |
| `Get_Measure_Delay` | `:MEASure:DELay?` |  | MEAS | unverified |
| `Get_Measure_Falltime` | `:MEASure:FALLtime?` |  | MEAS | unverified |
| `Get_Measure_Nwidth` | `:MEASure:NWIDth?` |  | MEAS | unverified |
| `Get_Measure_Overshoot` | `:MEASure:OVERshoot?` |  | MEAS | unverified |
| `Get_Measure_Phase` | `:MEASure:PHASe?` |  | MEAS | unverified |
| `Get_Measure_Preshoot` | `:MEASure:PREShoot?` |  | MEAS | unverified |
| `Get_Measure_Pwidth` | `:MEASure:PWIDth?` |  | MEAS | unverified |
| `Get_Measure_Risetime` | `:MEASURE:RISETIME?` |  | MEASURE | unverified |
| `Get_Measure_Show` | `:MEASure:SHOW?` |  | MEAS | unverified |
| `Get_Time_Stats_CH1` | `:MEASure:SOURce <source>;:MEASure:FREQuency?;:MEASure:PERiod?;:MEASure:DUTYcycle?;:MEASure:RISetime?` | D0 · D1 · D2 · D3 · D4 · D5 · D6 · D7 … | Channel 1 Measurements |  |
| `Get_Time_Stats_CH2` | `:MEASure:SOURce <source>;:MEASure:FREQuency?;:MEASure:PERiod?;:MEASure:DUTYcycle?;:MEASure:RISetime?` | D0 · D1 · D2 · D3 · D4 · D5 · D6 · D7 … | Channel 2 Measurements |  |
| `Get_Voltage_Stats_CH1` | `:MEASure:SOURce <source>;:MEASure:VPP?;:MEASure:VRMS?;:MEASure:VMAX?;:MEASure:VMIN?` | D0 · D1 · D2 · D3 · D4 · D5 · D6 · D7 … | Channel 1 Measurements |  |
| `Get_Voltage_Stats_CH2` | `:MEASure:SOURce <source>;:MEASure:VPP?;:MEASure:VRMS?;:MEASure:VMAX?;:MEASure:VMIN?` | D0 · D1 · D2 · D3 · D4 · D5 · D6 · D7 … | Channel 2 Measurements |  |
| `measure_1` | `:MEASure:SOURce CHANnel1;:MEASure:VPP?;:MEASure:VRMS?;:MEASure:FREQuency?` |  | MEASure | unverified |
| `measure_2` | `:MEASure:SOURce CHANnel2;:MEASure:VPP?;:MEASure:VRMS?;:MEASure:FREQuency?` |  | MEASure | unverified |
| `Get_Math_Statistics` | `:MEASure:SOURce FUNCtion;:MEASure:VPP?;:MEASure:VMAX?;:MEASure:VMIN?;:MEASure:VAVerage?` |  | Read statistics for the active Math function |  |
| `Get_Measure_Source` | `:MEASure:SOURce?` |  | MEAS | unverified |
| `Get_Measure_Tedge` | `:MEASure:TEDGe?` |  | MEAS | unverified |
| `Get_Measure_Tvalue` | `:MEASure:TVALue?` |  | MEAS | unverified |
| `Get_Measure_Vamplitude` | `:MEASure:VAMPlitude?` |  | MEAS | unverified |
| `Get_Measure_Vbase` | `:MEASure:VBASe?` |  | MEAS | unverified |
| `Get_Measure_Vtime` | `:MEASure:VTIMe?` |  | MEAS | unverified |
| `Get_Measure_Vtop` | `:MEASure:VTOP?` |  | MEAS | unverified |
| `Get_Measure_Xmax` | `:MEASure:XMAX?` |  | MEAS | unverified |
| `Get_Measure_Xmin` | `:MEASure:XMIN?` |  | MEAS | unverified |
| `Get_Probe_Skew` | `PROBe:SKEW?` |  | PROB | unverified |
| `Get_System_Date` | `:SYSTem:DATE?` |  | SYST | unverified |
| `Get_Error` | `SYSTem:ERRor?` |  | System Utilities |  |
| `Read_Error` | `:SYSTem:ERRor?` |  | Errors and ID |  |
| `Get_System_Lock` | `:SYSTem:LOCK?` |  | SYST | unverified |
| `Get_Setup` | `SYSTem:SETup?` |  | System Utilities |  |
| `Get_System_Time` | `:SYSTem:TIME?` |  | SYST | unverified |
| `Get_Timebase_Mode` | `:TIMebase:MODE?` |  | TIM | unverified |
| `Get_Timebase_Position` | `:TIMebase:POSition?` |  | TIM | unverified |
| `Get_Timebase_Range` | `:TIMebase:RANGe?` |  | TIM | unverified |
| `Get_Timebase_Reference` | `:TIMebase:REFerence?` |  | TIM | unverified |
| `Get_Timebase_Scale` | `:TIMebase:SCALe?` |  | TIM | unverified |
| `timebase_settings` | `:TIMebase:SCALe?;:TIMebase:POSition?` |  | TIMebase | unverified |
| `Get_Timebase_Window_Position` | `:TIMebase:WINDow:POSition?` |  | TIM | unverified |
| `Get_Timebase_Window_Range` | `:TIMebase:WINDow:RANGe?` |  | TIM | unverified |
| `Get_Timebase_Window_Scale` | `:TIMebase:WINDow:SCALe?` |  | TIM | unverified |
| `Get_Trigger_Can_Acknowledge` | `:TRIGger:CAN:ACKNowledge?` |  | TRIG | unverified |
| `Get_Trigger_Can_Pattern_Data` | `:TRIGger:CAN:PATTern:DATA?` |  | TRIG | unverified |
| `Get_Trigger_Can_Pattern_Id_Mode` | `:TRIGger:CAN:PATTern:ID:MODE?` |  | TRIG | unverified |
| `Get_Trigger_Can_Pattern_Id` | `:TRIGger:CAN:PATTern:ID?` |  | TRIG | unverified |
| `Get_Trigger_Can_Samplepoint` | `:TRIGger:CAN:SAMPlepoint?` |  | TRIG | unverified |
| `Get_Trigger_Can_Signal_Baudrate` | `:TRIGger:CAN:SIGNal:BAUDrate?` |  | TRIG | unverified |
| `Get_Trigger_Can_Source` | `:TRIGger:CAN:SOURce?` |  | TRIG | unverified |
| `Get_Trigger_Can_Trigger` | `:TRIGger:CAN:TRIGer?` |  | TRIG | unverified |
| `Get_Trigger_Coupling` | `:TRIGger:COUPling?` |  | TRIG | unverified |
| `Get_Trigger_Duration_Greaterthan` | `:TRIGger:DURation:GREaterthan?` |  | TRIG | unverified |
| `Get_Trigger_Duration_Lessthan` | `:TRIGger:DURation:LESSthan?` |  | TRIG | unverified |
| `Get_Trigger_Duration_Pattern` | `:TRIGger:DURation:PATTern?` |  | TRIG | unverified |
| `Get_Trigger_Duration_Qualifier` | `:TRIGger:DURation:QUALifier?` |  | TRIG | unverified |
| `Get_Trigger_Duration_Range` | `:TRIGger:DURation:RANGe?` |  | TRIG | unverified |
| `Get_Trigger_Edge_Level` | `:TRIGger:EDGE:LEVel?` |  | TRIG | unverified |
| `Get_Trigger_Edge_Slope` | `:TRIGger:EDGE:SLOPe?` |  | TRIG | unverified |
| `Get_Trigger_Edge_Source` | `:TRIGger:EDGE:SOURce?` |  | TRIG | unverified |
| `Get_Trigger_Glitch_Greaterthan` | `:TRIGger:GLITch:GREaterthan?` |  | TRIG | unverified |
| `Get_Trigger_Glitch_Lessthan` | `:TRIGger:GLITch:LESSthan?` |  | TRIG | unverified |
| `Get_Trigger_Glitch_Level` | `:TRIGger:GLITch:LEVel?` |  | TRIG | unverified |
| `Get_Trigger_Glitch_Polarity` | `:TRIGger:GLITch:POLarity?` |  | TRIG | unverified |
| `Get_Trigger_Glitch_Qualifier` | `:TRIGger:GLITch:QUALifier?` |  | TRIG | unverified |
| `Get_Trigger_Glitch_Range` | `:TRIGger:GLITch:RANGe?` |  | TRIG | unverified |
| `Get_Trigger_Glitch_Source` | `:TRIGger:GLITch:SOURce?` |  | TRIG | unverified |
| `Get_Trigger_Hfreject` | `:TRIGger:HFReject?` |  | TRIG | unverified |
| `Get_Trigger_Holdoff` | `:TRIGger:HOLDoff?` |  | TRIG | unverified |
| `Get_Trigger_Iic_Pattern_Address` | `:TRIGger:IIC:PATTern:ADDRess?` |  | TRIG | unverified |
| `Get_Trigger_Iic_Pattern_Data` | `:TRIGger:IIC:PATTern:DATA?` |  | TRIG | unverified |
| `Get_Trigger_Iic_Trigger_Qualifier` | `:TRIGger:IIC:TRIGger:QUALifer?` |  | TRIG | unverified |
| `Get_Trigger_Lin_Signal_Baudrate` | `:TRIGger:LIN:SIGNal:BAUDrate?` |  | TRIG | unverified |
| `Get_Trigger_Lin_Source` | `:TRIGger:LIN:SOURce?` |  | TRIG | unverified |
| `Get_Trigger_Lin_Trigger` | `:TRIGger:LIN:TRIGger?` |  | TRIG | unverified |
| `Get_Trigger_Mode` | `:TRIGger:MODE?` |  | TRIG | unverified |
| `trigger_settings` | `:TRIGger:MODE?;:TRIGger:EDGE:LEVel?;:TRIGger:EDGE:SOURce?` |  | TRIGger |  |
| `Get_Trigger_Nreject` | `:TRIGger:NREJect?` |  | TRIG | unverified |
| `Get_Trigger_Pattern` | `:TRIGger:PATTern?` |  | TRIG | unverified |
| `Get_Trigger_Reject` | `:TRIGger:REJect?` |  | TRIG | unverified |
| `Get_Trigger_Sequence_Count` | `:TRIGger:SEQuence:COUNt?` |  | TRIG | unverified |
| `Get_Trigger_Sequence_Find` | `:TRIGGER:SEQuence:FIND?` |  | TRIGGER | unverified |
| `Get_Trigger_Sequence_Reset` | `:TRIGGER:SEQuence:RESet?` |  | TRIGGER | unverified |
| `Get_Trigger_Sequence_Timebase` | `:TRIGGER:SEQuence:TIMer?` |  | TRIGGER | unverified |
| `Get_Trigger_Sequence_Trigger` | `:TRIGGER:SEQuence:TRIGger?` |  | TRIGGER | unverified |
| `Get_Trigger_Spi_Clock_Slope` | `:TRIGger:SPI:CLOCk:SLOPe?` |  | TRIG | unverified |
| `Get_Trigger_Spi_Clock_Timebase` | `:TRIGger:SPI:CLOCk:TIMeout?` |  | TRIG | unverified |
| `Get_Trigger_Spi_Frame` | `:TRIGger:SPI:FRAMing?` |  | TRIG | unverified |
| `Get_Trigger_Spi_Pattern_Data` | `:TRIGger:SPI:PATTern:DATA?` |  | TRIG | unverified |
| `Get_Trigger_Spi_Pattern_Width` | `:TRIGger:SPI:PATTern:WIDth?` |  | TRIG | unverified |
| `Get_Trigger_Spi_Source_Clock` | `:TRIGger:SPI:SOURce:CLOCk?` |  | TRIG | unverified |
| `Get_Trigger_Spi_Source_Data` | `:TRIGger:SPI:SOURce:DATA?` |  | TRIG | unverified |
| `Get_Trigger_Spi_Source_Frame` | `:TRIGger:SPI:SOURce:FRAMe?` |  | TRIG | unverified |
| `Get_Trigger_Sweep` | `:TRIGger:SWEep?` |  | TRIG | unverified |
| `Get_Trigger_Tv_Line` | `:TRIGger:TV:LINE?` |  | TRIG | unverified |
| `Get_Trigger_Tv_Mode` | `:TRIGger:TV:MODE?` |  | TRIG | unverified |
| `Get_Trigger_Tv_Polarity` | `:TRIGger:TV:POLarity?` |  | TRIG | unverified |
| `Get_Trigger_Tv_Source` | `:TRIGger:TV:SOURce?` |  | TRIG | unverified |
| `Get_Trigger_Tv_Standard` | `:TRIGger:TV:STANdard?` |  | TRIG | unverified |
| `Get_Trigger_Tv_Tvmode` | `:TRIGger:TV:TVMODE?` |  | TRIG | unverified |
| `Get_Trigger_Usb_Source_Dminus` | `:TRIGger:USB:SOURce:DMINus?` |  | TRIG | unverified |
| `Get_Trigger_Usb_Source_Dplus` | `:TRIGger:USB:SOURce:DPLus?` |  | TRIG | unverified |
| `Get_Trigger_Usb_Speed` | `:TRIGger:USB:SPEed?` |  | TRIG | unverified |
| `Get_Trigger_Usb_Trigger` | `:TRIGger:USB:TRIGger?` |  | TRIG | unverified |
| `Get_Waveform_Byteorder` | `:WAVeform:BYTeorder?` |  | WAV | unverified |
| `Get_Waveform_Count` | `:WAVeform:COUNt?` |  | WAV | unverified |
| `Get_Waveform_Data` | `WAVeform:DATA?` |  | Waveform Data Readbacks |  |
| `Get_Waveform_Format` | `:WAVeform:FORMat?` |  | WAV | unverified |
| `Get_Waveform_Points` | `:WAVeform:POINts?` |  | WAV | unverified |
| `Get_Preamble` | `WAVeform:PREamble?` |  | Waveform Data Readbacks |  |
| `waveform_1` | `:WAVeform:SOURce CHANnel1;:WAVeform:FORMat ASCii;:WAVeform:POINts 1000;:WAVeform:DATA?;:WAVeform:XORigin?;:WAVeform:XINCrement?` |  | WAVeform | unverified |
| `waveform_2` | `:WAVeform:SOURce CHANnel2;:WAVeform:FORMat ASCii;:WAVeform:POINts 1000;:WAVeform:DATA?;:WAVeform:XORigin?;:WAVeform:XINCrement?` |  | WAVeform | unverified |
| `Get_Waveform_Source` | `:WAVeform:SOURce?` |  | WAV | unverified |
| `Get_Waveform_Unsigned` | `:WAVeform:UNSigned?` |  | WAV | unverified |
| `Get_Waveform_View` | `:WAVeform:VIEW?` |  | WAV | unverified |
| `Get_Waveform_Xincrement` | `:WAVeform:XINCrement?` |  | WAV | unverified |
| `Get_Waveform_Xorigin` | `:WAVeform:XORigin?` |  | WAV | unverified |
| `Get_Waveform_Xreference` | `:WAVeform:XREFerence?` |  | WAV | unverified |
| `Get_Waveform_Yincrement` | `:WAVeform:YINCrement?` |  | WAV | unverified |
| `Get_Waveform_Yorigin` | `:WAVeform:YORigin?` |  | WAV | unverified |
| `Get_Waveform_Yreference` | `:WAVeform:YREFerence?` |  | WAV | unverified |

## `rig` — configures several arguments at once (1)

| Command | SCPI | Argument | Group | |
|---|---|---|---|---|
| `Setup_Trigger_Edge` | `:TRIGger:EDGE:SOURce <source>;:TRIGger:EDGE:SLOPe <slope>;:TRIGger:EDGE:LEVel <level>` | enum | Edge Trigger Config | unverified |

## `do` — executes an action; takes no value (106)

| Command | SCPI | Argument | Group | |
|---|---|---|---|---|
| `Do_Clear_Status` | `*CLS` |  | Actions and Toggles |  |
| `Do_Opc` | `*OPC` |  | Common | unverified |
| `Reset_Device` | `*RST` |  | Actions and Toggles |  |
| `Do_Trg` | `*TRG` |  | Common | unverified |
| `Do_Wai` | `*WAI` |  | Common | unverified |
| `Auto_Scale` | `:AUToscale` |  | Acquisition Control |  |
| `Autoscale` | `AUToscale` |  | Root Action Commands |  |
| `Do_Autoscale` | `:AUToscale` |  | Actions and Toggles |  |
| `Do_Channel_Bwlimit` | `:CHANNEL1:BWLIMIT` |  | CHANNEL | unverified |
| `Do_CH1_OFF` | `:CHANnel1:DISPlay OFF` |  | Actions and Toggles |  |
| `Do_CH1_ON` | `:CHANnel1:DISPlay ON` |  | Actions and Toggles |  |
| `Do_Channel_Offset` | `:CHANNEL1:OFFSET` |  | CHANNEL | unverified |
| `Do_Channel_Probe` | `:CHANNEL1:PROBE` |  | CHANNEL | unverified |
| `Do_CH2_OFF` | `:CHANnel2:DISPlay OFF` |  | Actions and Toggles |  |
| `Do_CH2_ON` | `:CHANnel2:DISPlay ON` |  | Actions and Toggles |  |
| `Do_Channel_Skew` | `CHANnel2:SKEW` |  | CHAN | unverified |
| `Do_Channel_Activity` | `CHANnel:ACTivity` |  | CHAN | unverified |
| `Do_Channel_Math` | `CHANnel:MATH` |  | CHAN | unverified |
| `Do_Channel_Threshold` | `CHANnel:THReshold` |  | CHAN | unverified |
| `Digitize_Channel` | `DIGitize <chan>` |  | Root Action Commands |  |
| `Do_Clear_Display` | `:DISPlay:CLEar` |  | Actions and Toggles |  |
| `Do_Display_Column` | `DISPlay:COLumn` |  | DISP | unverified |
| `Do_Display_Connect` | `DISPlay:CONNect` |  | DISP | unverified |
| `Do_Display_Grid` | `DISPlay:GRID` |  | DISP | unverified |
| `Do_Display_Invert` | `DISPlay:INVerse` |  | DISP | unverified |
| `Do_Display_Line` | `DISPLay:LINE` |  | DISPL | unverified |
| `Do_Display_Order` | `DISPlay:ORDer` |  | DISP | unverified |
| `Do_Display_Pixel` | `DISPlay:PIXel` |  | DISP | unverified |
| `Do_Display_Position` | `DISPlay:POSition` |  | DISP | unverified |
| `Do_Display_Row` | `DISPlay:ROW` |  | DISP | unverified |
| `Do_Display_Text` | `DISPlay:TEXT` |  | DISP | unverified |
| `Do_External_Input` | `EXTernal:INPut` |  | EXT | unverified |
| `Do_External_Pmode` | `EXTernal:PMODe` |  | EXT | unverified |
| `Do_External_Protection_Clear` | `:EXTernal:PROTection:CLEAR` |  | EXT | unverified |
| `Do_Math_OFF` | `:FUNCtion:DISPlay OFF` |  | Math Display Controls |  |
| `Do_Math_ON` | `:FUNCtion:DISPlay ON` |  | Math Display Controls |  |
| `Do_Function_Move` | `FUNCtion:MOVE` |  | FUNC | unverified |
| `Do_Function_Peaks` | `FUNCtion:PEAKs` |  | FUNC | unverified |
| `Set_Source_CH1` | `:FUNCtion:SOURce CHANnel1` |  | Source Selection |  |
| `Set_Source_CH2` | `:FUNCtion:SOURce CHANnel2` |  | Source Selection |  |
| `Do_Function_View` | `FUNCtion:VIEW` |  | FUNC | unverified |
| `Do_Hardcopy_Address` | `HARDcopy:ADDRess` |  | HARD | unverified |
| `Do_Hardcopy_Destination` | `:HARDcopy:DESTination` |  | HARD | unverified |
| `Do_Hardcopy_Device` | `HARDcopy:DEVice` |  | HARD | unverified |
| `Do_Marker_Tdelta` | `MARKer:TDELta` |  | MARK | unverified |
| `Do_Marker_Vdelta` | `MARKer:VDELta` |  | MARK | unverified |
| `Do_Measure_Clear` | `MEASure:CLEar` |  | MEAS | unverified |
| `Do_Measure_Lower` | `MEASure:LOWer` |  | MEAS | unverified |
| `Do_Measure_Risetime` | `:MEASure:RISEtime` |  | MEAS | unverified |
| `Do_Measure_Scratch` | `MEASure:SCRatch` |  | MEAS | unverified |
| `Do_Measure_Tdelta` | `MEASure:TDELta` |  | MEAS | unverified |
| `Do_Measure_Threshold` | `MEASure:THResholds` |  | MEAS | unverified |
| `Do_Measure_Tmax` | `MEASure:TMAX` |  | MEAS | unverified |
| `Do_Measure_Tmin` | `MEASure:TMIN` |  | MEAS | unverified |
| `Do_Measure_Tstart` | `MEASure:TSTArt` |  | MEAS | unverified |
| `Do_Measure_Tstop` | `MEASure:TSTOp` |  | MEAS | unverified |
| `Do_Measure_Tvolt` | `MEASure:TVOLt` |  | MEAS | unverified |
| `Do_Measure_Upper` | `MEASure:UPPer` |  | MEAS | unverified |
| `Do_Measure_Vdelta` | `MEASure:VDELta` |  | MEAS | unverified |
| `Do_Measure_Vstart` | `MEASure:VSTArt` |  | MEAS | unverified |
| `Do_Measure_Vstop` | `MEASure:VSTOp` |  | MEAS | unverified |
| `Do_Protection_Clear` | `:PROTection:CLEAR` |  | PROT | unverified |
| `Do_Run` | `:RUN` |  | Actions and Toggles |  |
| `Run` | `RUN` |  | Root Action Commands |  |
| `Do_Single` | `:SINGle` |  | Actions and Toggles |  |
| `Single` | `SINGle` |  | Root Action Commands |  |
| `Do_Stop` | `:STOP` |  | Actions and Toggles |  |
| `Stop` | `STOP` |  | Root Action Commands |  |
| `Do_System_Key` | `SYSTem:KEY` |  | SYST | unverified |
| `Do_Timebase_Delay` | `TIM:DEL` |  | TIM | unverified |
| `Do_Timebase_Window` | `TIMebase:WINDow` |  | TIM | unverified |
| `Do_Trigger_Advanced` | `TRIGger:ADVanced` |  | TRIG | unverified |
| `Do_Trigger_Can` | `TRIGger:CAN` |  | TRIG | unverified |
| `Do_Trigger_Can_Pattern` | `TRIGger:CAN:PATTern` |  | TRIG | unverified |
| `Do_Trigger_Can_Signal` | `TRIGger:CAN:SIGNal` |  | TRIG | unverified |
| `Do_Trigger_Duration` | `TRIGger:DURation` |  | TRIG | unverified |
| `Do_Trigger_Duration_Greaterthan` | `:TRIGGER:DURation:GREaterthan` |  | TRIGGER | unverified |
| `Do_Trigger_Duration_Lessthan` | `:TRIGGER:DURation:LESSthan` |  | TRIGGER | unverified |
| `Do_Trigger_Edge` | `TRIGger:EDGE` |  | TRIG | unverified |
| `Force_Trigger` | `:TRIGger:FORCe` |  | Root Action Commands | unverified |
| `Do_Trigger_Glitch` | `TRIGger:GLITch` |  | TRIG | unverified |
| `Do_Trigger_Glitch_Greaterthan` | `:TRIGGER:GLITch:GREaterthan` |  | TRIGGER | unverified |
| `Do_Trigger_Glitch_Lessthan` | `:TRIGGER:GLITch:LESSthan` |  | TRIGGER | unverified |
| `Do_Trigger_Iic` | `TRIGger:IIC` |  | TRIG | unverified |
| `Do_Trigger_Iic_Pattern` | `TRIGger:IIC:PATTern` |  | TRIG | unverified |
| `Do_Trigger_Iic_Source` | `:TRIGger:IIC:SOURce` |  | TRIG | unverified |
| `Do_Trigger_Iic_Trigger` | `TRIGger:IIC:TRIGger` |  | TRIG | unverified |
| `Do_Trigger_Level` | `:TRIGGER:LEVEL` |  | TRIGGER | unverified |
| `Do_Trigger_Lin` | `TRIGger:LIN` |  | TRIG | unverified |
| `Do_Trigger_Lin_Signal` | `TRIGger:LIN:SIGNal` |  | TRIG | unverified |
| `Do_Trigger_Sequence` | `TRIGger:SEQuence` |  | TRIG | unverified |
| `Do_Trigger_Sequence_Edge` | `:TRIGger:SEQuence:EDGE` |  | TRIG | unverified |
| `Do_Trigger_Sequence_Pattern` | `:TRIGger:SEQuence:PATTern` |  | TRIG | unverified |
| `Do_Trigger_Slope` | `:TRIGGER:SLOPE` |  | TRIGGER | unverified |
| `Do_Trigger_Spi` | `TRIGger:SPI` |  | TRIG | unverified |
| `Do_Trigger_Spi_Clock` | `TRIGger:SPI:CLOCk` |  | TRIG | unverified |
| `Do_Trigger_Spi_Pattern` | `TRIGger:SPI:PATTERN` |  | TRIG | unverified |
| `Do_Trigger_Spi_Source` | `TRIGger:SPI:SOURce` |  | TRIG | unverified |
| `Do_Trigger_Threshold` | `TRIGger:THReshold` |  | TRIG | unverified |
| `Do_Trigger_Tv` | `TRIGger:TV` |  | TRIG | unverified |
| `Do_Trigger_Tv_Field` | `TRIGger:TV:FIELd` |  | TRIG | unverified |
| `Do_Trigger_Tv_Tvhfrej` | `TRIGger:TV:TVHFrej` |  | TRIG | unverified |
| `Do_Trigger_Tv_Tvmode` | `TRIGger:TV:TVMode` |  | TRIG | unverified |
| `Do_Trigger_Tv_Vir` | `TRIGger:TV:VIR` |  | TRIG | unverified |
| `Do_Trigger_Usb` | `TRIGger:USB` |  | TRIG | unverified |
| `Do_Trigger_Usb_Source` | `TRIGger:USB:SOURce` |  | TRIG | unverified |
