# SolPipLog ![solpiplog](solpiplog.gif)

**Logger for the PIP Inverter series ( USB + RS232 version) + BMV Battery Monitor** 
* Voltronic Axpert, Mppsolar PIP, Voltacon, Effekta, and other branded Oems
* Victron Battery Monitor BMV700 and BMV702

* want to support me ? [support](https://paypal.me/solpiplog)

- update at work.....123
- latest version 2.0.0 version Phoenix 02/2017 
- working on 32bit UBUNTU / MATE.
- working on Raspberry Pi2/Pi3 version. link for [Raspberry Image](https://my.pcloud.com/publink/show?code=XZ0yMz7ZvssSH2MOuYzA1giJh5JM7f8O1zB7)
- logs data from BMV battery monitor to [Emoncms](https://emoncms.org) 
- does not work on Windows.
- sends data to [Emoncms](https://emoncms.org) 

 Emoncms is an open-source web application for processing, logging and visualising energy, temperature and other environmental data and is part of the [OpenEnergyMonitor project](http://openenergymonitor.org).

- sends data to [PVOutput](http://www.pvoutput.org).

 PVOutput is a free service for sharing and comparing PV output data.

## Install
 * For **RASPBERRY** users. Copy folder **"sol"** to yout **"/home/pi"** directory. Execute "setup.sh" which is inside "sol" folder
 * For **UBUNTU USERS** copy file **"solpiplog.rules"** to your **"/etc/udev/rules.d"** directory. That way you dont have to excecute it as root
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
 * choose autoload config and start and press on Save ( if you restart SolPipLog it loads the config file and runs. )
   
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

* 30 = Year for displaying lastest update
* 31 = Month
* 32 = Day
* 33 = Hour
* 34 = Minute
* 35 = Second

* 

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


## Version


follow on http://www.photovoltaikforum.com/datenlogger-f5/usb-datenlogger-fuer-pip-serie-solpiplog-t114101.html
raspberry image available.
image based on RASPBIAN STRETCH, SAMBA installed ( folder solpiplog visible on local network ), RealVNC installed,
username and password are default ones from STRETCH image.
* 2.0.0 * Phoenix version
	* support for parallel inverter reading 4 at once
	* ability to change node
	* layout changed. cosmetic alterations.
	* 			
* 1.5.0 * Primavera version
	* support for Inverter with 2 MPPT
	* logs aditional parameter for BMV702
	* Sends UDP datagramm to a Server / for example to a Loxone Smart Home server
	* autoload config and Start possible.
	* bug crc errors solved
	* solved timeout on 2MPPT versions solved
* 1.4.9a* rik_man UDP version
* 1.4.9 * tealc_hr internal forum release
* 1.4.8 * 03/2017 new  change BULK and FLOAT
* 1.4.7 * Vollkorn changed how to Switch to UTI/SOL.
* 1.4.6 * BennyHH BMV logging without PIP online
* 1.4.5 * agenturrene v4 change charger priority
* 1.4.4 * agenturrene v3 switching SOC error
* 1.4.3 * agenturrene v2 faster bmv detection
* 1.4.2 * agenturrene v1 two MPPT version
* 1.4.1 * 11/2016 RS232 public release
	change on SOC activated.
	Changes inverter to UTI or SBU based on SOC

* 1.4.0 * Vollkorn release RS232 support for Inverter
	bugfixes, layout changed.
* 1.3.1 * BennyHH Soc version internal release
* 1.3.0	* 10/2016 NEW  BMV Battery Monitor log parameter send to EmonCMS on Node 20
  	* Key 1 :  Battery voltage mV
  	* Key 2 : Battery current mA
  	* Key 3 : Instantaneous Power W
  	* Key 4 : Consumed Amp Hours mAh
  	* Key 5 : State-of-Charge
  	* Key 6 : Time-to-go in minutes
	* Key 8 : Alarm status ON/OFF
	* Key 25:  Relay status ON/OFF

* 1.2.6 * BennyHH v3 internal test
	* new parameter 30 : Year
	* new parameter 31 : Month
	* new parameter 32 : Day
	* new parameter 33 : Hour
	* new parameter 34 : Minute
	* new parameter 35 : Seconds
* 1.2.5 * BennyHH v2 internal test
	* Added parameter 18 Line Mode
	* Added parameter 19 Battery Mode
	* Added parameter 20 Fault Mode
	* add detection if internet connection available

* 1.2.4 -* bug timer overflow
	* changes on workflow for slow machines
	* rewritten parser
	* cosmetic changes
	* raspberry 2 version adaptation
	* a lot of bugs removed

* 1.2.3.alpha - BennyHH version

* 1.2.2 - * bug timeout problems on slow machines increased to 5 seconds
	* log screen . showing all errors.
 
* 1.2.1 - removed change by watt ( debug version )
	- updated logo
	- bug* Connect button without focus after clicking manual Disconnect

* 1.2 - fist public release


