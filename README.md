# SolPipLog

Logger for the PIP Inverter series ( USB version )

- working on 32bit UBUNTU / MATE.
- no Windows version yet
- sends data to [Emoncms](https://emoncms.org) 

 Emoncms is an open-source web application for processing, logging and visualising energy, temperature and other environmental data and is part of the [OpenEnergyMonitor project](http://openenergymonitor.org).

- sends data to [PVOutput](http://www.pvoutput.org).


## Install
 * copy file **"solpiplog.rules"** to your **"/etc/udev/rules.d/"** directory. That way you dont have to excecute it as root
 * make **solpiplog** executable with
   * **sudo chmod +x solpiplog** or 
   * change it with graphical interface inside of Ubuntu / Mate. right click on file - properties - permissions tab - tick execute allow excecuting file as program
   

