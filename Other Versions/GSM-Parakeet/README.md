# GSM / Parakeet Version

# Experimental Version - has not been tested yet
To order the PCB click [here](https://oshpark.com/shared_projects/pyIarV64).

This version uses a GSM module (SIM800L) instead of bluetooth. Check the [Parakeet project](https://jamorham.github.io/) for more info.

I had to switch to the TP4056 Charging IC because it has more power and is cheaper.


## Features:

- The board uses a TP4056 battery charging ic with a maximum charging power of 1000mA
- SIM800L Module sends the CGM data directly to the cloud
- Battery can be soldered directly on the PCB (2.54mm header) or via a JST-2 connector (2mm pitch)
- Charging Status LED, Red = charging; Green = Full
- 4 ways to connect the battery: 
- - JST-2 (sparkfun batteries)
- - JST-XH (ebay batteries)
- - 2.54mm pitch screw-in connector
- - solder the wires directly

## Changelog
rev.1.0 - added JST-XH footprint, improoved pcb traces and vias

rev.0.9 - fixed SIM800L footprint, improoved pcb traces and vias

rev.0.8 - first version ready to manufacture


# Components


Most can be sourced from eBay


- SIM800L GSM Module
- 1x Polulu Wixel
- TP4056 Li Charging IC
- 2x 10μf Capacitors
- 1x 1.2kΩ Resistor (RPROG - 1.2kΩ=1000mA - Depends on Charging current - Check table below)
- 2x 330Ω Resistor
- 2x 1206 LED (1 Red and 1 Green)
- 1x [Micro USB Connector Female 4Legs](http://www.ebay.com/itm/10Pcs-Micro-USB-Type-B-Female-Socket-4-Vertical-Legs-For-Solder-Connectors-/351570406777?hash=item51db3aad79:g:UUwAAOSwu-BWOscw)
- 1x micro switch MSK-12C02
- 1x LiPo/Li-ion Battery (I recommend using a LiPo battery)
- 1x [JST-2 connector 2mm pitch](https://www.sparkfun.com/products/8612) (optional - your battery needs to have the mating connector - sparkfun sells compatible batteries, or buy the connector separately and crimp it on your battery)
- 1x JST-XH 2-pin connector (optional - only if your battery has this type of connector or you plan on crimping your own)

# Setting the charging current

You can individually set the charging current. Just change the RPROG resistor to the value you want.
The charging Current should be set dependent on the battery used. Always use a charging current equal or lower than the battery capacity.

|RPROG (kΩ)|IBAT(mA)| 
|:--------:|:------:|
|10        |130     |
|5         |250     |
|4         |300     |
|3         |400     |
|2         |580     |
|1.66      |690     |
|1.5       |780     |
|1.33      |900     |
|1.2       |1000    |


## Schematics:

![Schematics](https://github.com/mzst123/Xdrip-Lipo-Board/blob/master/Other%20Versions/GSM-Parakeet/img_parakeet-sch.png)


## Pictures:


![Top View](https://644db4de3505c40a0444-327723bce298e3ff5813fb42baeefbaa.ssl.cf1.rackcdn.com/4a49c66479cc872754cc7636690bfe43.png)


![Bottom View](https://644db4de3505c40a0444-327723bce298e3ff5813fb42baeefbaa.ssl.cf1.rackcdn.com/ba2c8e37a4952ce03b12c1a464a7485f.png)