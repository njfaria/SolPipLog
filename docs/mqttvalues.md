## Values sent over MQTT

- solpiplog/pip/acin
- solpiplog/pip/acout
- solpiplog/pip/acoutva
- solpiplog/pip/acoutw
- solpiplog/pip/load
- solpiplog/pip/battv
- solpiplog/pip/battchrg
- solpiplog/pip/battcappa
- solpiplog/pip/heatsinktemp
- solpiplog/pip/pvibatt
- solpiplog/pip/pvvolt
- solpiplog/pip/battvscc
- solpiplog/pip/batdischrg
- solpiplog/pip/pvchargew
- solpiplog/pip/status
- solpiplog/pip/status2
- solpiplog/pip/masterstatus

- solpiplog/bmv/soc
- solpiplog/bmv/volt
- solpiplog/bmv/ampere
- solpiplog/bmv/consumedah
- solpiplog/bmv/watt
- solpiplog/bmv/relay
- solpiplog/bmv/h1
- solpiplog/bmv/h2
- solpiplog/bmv/h3
- solpiplog/bmv/h4
- solpiplog/bmv/h5
- solpiplog/bmv/h6
- solpiplog/bmv/h7
- solpiplog/bmv/h8
- solpiplog/bmv/h9
- solpiplog/bmv/h10
- solpiplog/bmv/h11
- solpiplog/bmv/h12
- solpiplog/bmv/h15
- solpiplog/bmv/h16
- solpiplog/bmv/h17
- solpiplog/bmv/h18
- solpiplog/bmv/timetogo
                     
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
- solpiplog/pip/solar1ampere
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
- solpiplog/pip/batpowerdir
- solpiplog/pip/dcacpowerdir
- solpiplog/pip/linepowerdir
- solpiplog/pip/workingmode
                                                                          



## Values changable over MQTT  
- solpiplog/pip/status/set with payload uti, sol, sbu
	for example: solpiplog/pip/status/set uti
	to change to grid
- solpiplog/pip/status/set with payload 0, 1, 2, 3 for charger settings  

## Values of Inverter status ( not for hybrid at the moment )
- solpiplog/pip/status
- solpiplog/pip/status2
- solpiplog/pip/masterstatus


                                                                         
