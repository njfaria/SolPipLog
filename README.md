# SolPipLog ![solpiplog](solpiplog.gif)

**Logger for the PIP Inverter series ( USB + RS232 version) + BMV Battery Monitor** 
* Voltronic Axpert, Mppsolar PIP, Voltacon, Effekta, and other branded Oems
* Victron Battery Monitor BMV700 and BMV702

* want to support me ? [support](https://paypal.me/solpiplog)

- 
- latest version 2.2.0 version Phoenix 04/2019 
- working on Raspberry Pi2/Pi3 version. link for [Raspberry Image](https://my.pcloud.com/publink/show?code=XZ0yMz7ZvssSH2MOuYzA1giJh5JM7f8O1zB7)
- logs data from BMV battery monitor to [Emoncms](https://emoncms.org) 
- sends data to [Emoncms](https://emoncms.org) 

 Emoncms is an open-source web application for processing, logging and visualising energy, temperature and other environmental data and is part of the [OpenEnergyMonitor project](http://openenergymonitor.org).

- sends data to [PVOutput](http://www.pvoutput.org).

 PVOutput is a free service for sharing and comparing PV output data.

## Install
 * For **RASPBERRY** users. Copy folder **"sol"** to yout **"/home/pi"** directory. Execute "setup.sh" which is inside "sol" folder
 * make **solpiplog** executable with
   * **sudo chmod +x solpiplog** or 
   * change it with graphical interface inside of Ubuntu / Mate. Right click on file - properties - permissions tab - tick execute allow excecuting file as program
   * problably you dont even need to do it, if i dont forget to make it executable :) 
 * create an account on [Emoncms](https://emoncms.org) or install **Emoncms** on your own server. 
 * optional: create an account on [PVOutput](http://www.pvoutput.org).
 * configure **SolPipLog** with your Emoncms API-Key
 * optional configure **SolPipLog** with your PVOutput SystemID and API-Key.
 * choose autoload config and start and press on Save ( if you restart SolPipLog it loads the config file and runs. )
   
## [Values sent to Emoncms](https://github.com/njfaria/SolPipLog/docs/emoncmsvalues.md)

## [Values sent over MQTT](https://github.com/njfaria/SolPipLog/docs/mqttvalues.md)

## [Version](https://github.com/njfaria/SolPipLog/docs/version.md)
* latest version 2.2.0

follow on http://www.photovoltaikforum.com/datenlogger-f5/usb-datenlogger-fuer-pip-serie-solpiplog-t114101.html
raspberry image available.
image based on RASPBIAN STRETCH, RealVNC installed,
username:pi
password:solpiplog
 
