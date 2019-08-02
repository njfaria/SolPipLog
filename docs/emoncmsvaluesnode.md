## Values sent to Emoncms with Node

Following values are sent to *Emoncms* and displayed as Node 30 with Key from 1-20 and 30-35

* 1  = AC_IN_V
* 2  = AC_IN_HZ
* 3  = AC_OUT_V
* 4  = AC_OUT_HZ
* 5  = AC_OUT_VA
* 6  = AC_OUT_W
* 7  = AC_OUT_LOAD_PERCENT
* 8  = BUS_V
* 9  = BATT_V
* 10 = BATT_CHRG
* 11 = BATT_CAPACITY_PERCENT
* 12 = HEATSINK_TEMP
* 13 = PV_I_BATT
* 14 = PV_V
* 15 = BATT_V_SCC
* 16 = BATT_DISCHRG_I
* 17 = PV Charging Power
* 18 = Line Mode ( 0 or 1 )  Link Led Widget for visualization
* 19 = Battery Mode ( 0 or 1 ) Link Led Widget for visualization
* 20 = Fault Mode ( 0 or 1 )  Link Led Widget for visualization

* 30 = Year for displaying lastest update
* 31 = Month
* 32 = Day
* 33 = Hour
* 34 = Minute
* 35 = Second

**New since v 1.4.9 support for Inverter with two/three MPPT displayed as Node 31 with following Keys:**

* 1 =  PV2 current A
* 2 =  PV2 volt V
* 3 =  batt volt scc2 V
* 4 =  PV power2 W
* 5 =  device status
* 6 =  AC charge current A
* 7 =  AC charge power W
* 8 =  PV3 current A
* 9 =  PV3 voltage V
* 10 = batt volt scc3 V
* 11 = PV power3 W
* 12 = PV total W


* 30 = Year for displaying lastest update
* 31 = Month
* 32 = Day
* 33 = Hour
* 34 = Minute
* 35 = Second
* 36 = Days since online
* 37 = Hours since Online	
* 38 = device status	
* 39 = device status2

* Inv1 01 Serial number
* Inv1 02 mode	
* Inv1 09 AC Out Power
* Inv1 11 Battery Voltage
* Inv1 12 Battery Charge A
* Inv1 17 TOTAL AC OUT W	
* Inv1 25 PV Input A	
* Inv1 26 Battery discharge A	
* Inv2 01 Serial number
* Inv2 02 mode	
* Inv2 09 AC Out Power
* Inv2 11 Battery Voltage
* Inv2 12 Battery Charge A
* Inv2 17 TOTAL AC OUT W	
* Inv2 25 PV Input A	
* Inv2 26 Battery discharge A	
* Inv3 01 Serial number
* Inv3 02 mode	
* Inv3 09 AC Out Power
* Inv3 11 Battery Voltage
* Inv3 12 Battery Charge A
* Inv3 17 TOTAL AC OUT W	
* Inv3 25 PV Input A	
* Inv3 26 Battery discharge A	
* Inv4 01 Serial number
* Inv4 02 mode	
* Inv4 09 AC Out Power
* Inv4 11 Battery Voltage
* Inv4 12 Battery Charge A
* Inv4 17 TOTAL AC OUT W	
* Inv4 25 PV Input A	
* Inv4 26 Battery discharge A	


**BMV Battery Monitor displayed as Node 20 with following Keys:**
* 1 = Battery voltage mV
* 2 = Battery current mA
* 3 = Instantaneous Power W
* 4 = Consumed amp Hours mAh
* 5 = State-of-Charge
* 6 = Time-To-Go in minutes
* 8 = Alarm status (ON/OFF) one for ON and zero for OFF
* 10 = Auxiliary (starter) voltage  ## only with BMV-702
* 11 = mid point voltage in mV
* 12 = mid point deviation 
* 25 = Relay status (ON/OFF)
 
## Values sent to PVOutput
Following values are sent to *PVOutput*

* AC_OUT_V
* AC_OUT_W
* PV Charging Power


