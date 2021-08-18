## Values sent over MQTT
- solpiplog/pip/acin
- solpiplog/pip/acinhz
- solpiplog/pip/acout
- solpiplog/pip/acinhz
- solpiplog/pip/acoutva
- solpiplog/pip/acoutw
- solpiplog/pip/battdischrg
- solpiplog/pip/battcappa
- solpiplog/pip/battchrg
- solpiplog/pip/battv
- solpiplog/pip/battvscc
- solpiplog/pip/bulk
- solpiplog/pip/busv
- solpiplog/pip/charge
- solpiplog/pip/devicestatus
- solpiplog/pip/float
- solpiplog/pip/heatsinktemp
- solpiplog/pip/load
- solpiplog/pip/masterstatus
- solpiplog/pip/maxcharge
- solpiplog/pip/pv2chargew
- solpiplog/pip/pv2ibatt
- solpiplog/pip/pv2volt
- solpiplog/pip/pvchargew
- solpiplog/pip/pvibatt
- solpiplog/pip/pvvolt
- solpiplog/pip/socactive
- solpiplog/pip/socvalue
- solpiplog/pip/status
- solpiplog/pip/status2
- solpiplog/pip/totalsolarw

                     
## P18 Hybrid Inverter

- solpiplog/pip/acin
- solpiplog/pip/acout
- solpiplog/pip/acoutva
- solpiplog/pip/acoutW
- solpiplog/pip/load
- solpiplog/pip/battv
- solpiplog/pip/battchrg
- solpiplog/pip/battcappa
- solpiplog/pip/heatsinktemp
- solpiplog/pip/pv1w
- solpiplog/pip/pv2w
- solpiplog/pip/pv1volt
- solpiplog/pip/pv2volt
- solpiplog/pip/dailywh
           
## P17 Hybrid Inverter

- solpiplog/pip/solar1volt
- solpiplog/pip/solar2volt
- solpiplog/pip/solar1ampere
- solpiplog/pip/solar2ampere
- solpiplog/pip/battvoltage
- solpiplog/pip/battcappa
- solpiplog/pip/battcurrent
- solpiplog/pip/acinrv
- solpiplog/pip/acinrfreq
- solpiplog/pip/acoutrv
- solpiplog/pip/acoutrfreq
- solpiplog/pip/innertemp
- solpiplog/pip/solar1power
- solpiplog/pip/solar2power
- solpiplog/pip/acoutpower
- solpiplog/pip/solar1status
- solpiplog/pip/solar2status
- solpiplog/pip/batpowerdir
- solpiplog/pip/dcacpowerdir
- solpiplog/pip/linepowerdir
- solpiplog/pip/workingmode

## Parallel inverter
_up to 7 inverter ( pip1 pip2 and so on )_
- solpiplog/pip1/serial
- solpiplog/pip1/mode
- solpiplog/pip1/acin
- solpiplog/pip1/acout
- solpiplog/pip1/acoutva
- solpiplog/pip1/acoutw
- solpiplog/pip1/load
- solpiplog/pip1/battv
- solpiplog/pip1/battchrg
- solpiplog/pip1/battdischrg
- solpiplog/pip1/battcappa
- solpiplog/pip1/totalacoutw
- solpiplog/pip1/pvinputvolt
- solpiplog/pip1/totalcharginga
- solpiplog/pip1/totalacoutva
- solpiplog/pip1/pvinputcurrentforbat



## Values changeable over MQTT  
- **solpiplog/pip/status/set** with payload **uti**, **sol**, **sbu**, 
payloads **aut**, **onl**, **eco** for KING inverter
	for example: **solpiplog/pip/status/set uti** to change to grid
- **solpiplog/pip/charger/set** with payload **0**, **1**, **2**, **3** for charger settings
- **solpiplog/pip/equalize/set** with payload **start** or **stop**
for inverter supporting equalize.
- **solpiplog/pip/timesource/set** and payload **on** or **off** 
-  **solpiplog/pip/timecharge/set** and payload **on** or **off** 

- **solpiplog/pip/maxcharge/set** and payloads **2**, **10**, **20**, **30**, **40**, **50**, **60**
- **solpiplog/pip/profile/set** and payload **1**, **2**
 


## Values of Inverter status ( not for hybrid at the moment )
- solpiplog/pip/status
- solpiplog/pip/status2
- solpiplog/pip/masterstatus


                                                                         
