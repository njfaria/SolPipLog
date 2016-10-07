# SolPipLog ![solpiplog](solpiplog.gif)

**Logger for the PIP Inverter series ( USB version ) + BMV Battery Monitor** 

- latest version 1.3.0 10/2016
- working on 32bit UBUNTU / MATE.
- working on Raspberry Pi2 version
- logs data from BMV battery monitor to [Emoncms](https://emoncms.org) 
- no Windows version yet
- sends data to [Emoncms](https://emoncms.org) 

 Emoncms is an open-source web application for processing, logging and visualising energy, temperature and other environmental data and is part of the [OpenEnergyMonitor project](http://openenergymonitor.org).

- sends data to [PVOutput](http://www.pvoutput.org).

 PVOutput is a free service for sharing and comparing PV output data.

## Install
 * copy file **"solpiplog.rules"** to your **"/etc/udev/rules.d"** directory. That way you dont have to excecute it as root
 * from your terminal window, inside the folder where the file is **sudo cp solpiplog.rules /etc/udev/rules.d** 
 * unplug usb cable and replug
 * make **solpiplog** executable with
   * **sudo chmod +x solpiplog** or 
   * change it with graphical interface inside of Ubuntu / Mate. Right click on file - properties - permissions tab - tick execute allow excecuting file as program
   * problably you dont even need to do it, if i dont forget to make it executable :) 
 * create an account on [Emoncms](https://emoncms.org) or install **Emoncms** on your own server. 
 * optional: create an account on [PVOutput](http://www.pvoutput.org).
 * configure **SolPipLog** with your Emoncms API-Key
  * optional configure **SolPipLog** with your PVOutput SystemID and API-Key.
  
## Values sent to Emoncms

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

* 30 = Year         for displaying lastest update 
* 31 = Month
* 32 = Day
* 33 = Hour
* 34 = Minute
* 35 = Second

New since v 1.3.0 BMV Battery Monitor displayed as Node 20 with following Keys:

* 1 = Battery voltage mV
* 2 = Battery current mA
* 3 = Instantaneous Power W
* 4 = Consumed amp Hours mAh
* 5 = State-of-Charge
* 6 = Time-To-Go in minutes
* 8 = Alarm status (ON/OFF) one for ON and zero for OFF
* 25 = Relay status (ON/OFF)



## Values sent to PVOutput
Following values are sent to *PVOutput*

* AC_OUT_V
* AC_OUT_W
* PV Charging Power

## Version

1.3.0 -* 10/2016 NEW  BMV Battery Monitor log parameter send to EmonCMS on Node 20
	* Key 1 :  Battery voltage mV
	* Key 2 : Battery current mA
	* Key 3 : Instantaneous Power W
	* Key 4 : Consumed Amp Hours mAh
	* Key 5 : State-of-Charge
	* Key 6 : Time-to-go in minutes
	* Key 8 : Alarm status ON/OFF
	* Key 25:  Relay status ON/OFF

1.2.6 -* BennyHH v3 internal test
	* new parameter 30 : Year
	* new parameter 31 : Month
	* new parameter 32 : Day
	* new parameter 33 : Hour
	* new parameter 34 : Minute
	* new parameter 35 : Seconds
1.2.5 - * BennyHH v2 internal test
	* Added parameter 18 Line Mode
	* Added parameter 19 Battery Mode
	* Added parameter 20 Fault Mode
	* add detection if internet connection available

1.2.4 -* bug timer overflow
	* changes on workflow for slow machines
	* rewritten parser
	* cosmetic changes
	* raspberry 2 version adaptation
	* a lot of bugs removed

1.2.3.alpha - BennyHH version

1.2.2 - * bug timeout problems on slow machines increased to 5 seconds
	* log screen . showing all errors.
           
1.2.1 - removed change by watt ( debug version )
	- updated logo
	- bug* Connect button without focus after clicking manual Disconnect

1.2 - fist public release


