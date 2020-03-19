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

- solpiplog/bmv/soc
- solpiplog/bmv/volt
- solpiplog/bmv/ampere
- solpiplog/bmv/consumedah
- solpiplog/bmv/watt
- solpiplog/bmv/relay
- solpiplog/bmv/h1
- solpiplog/bmv/h2
- solpiplog/bmv/h17
- solpiplog/bmv/h18

## Values changable over MQTT  
- solpiplog/pip/status/set with payload uti, sol, sbu
	for example: solpiplog/pip/status/set uti
	to change to grid
- solpiplog/pip/status/set with payload 0, 1, 2, 3 for charger settings                                                                           
