# Xdrip-Lipo-Board
Xdrip on a printed circuit board

Here you can find the Eagle files for the Xdrip-Lipo-Board

You can also order the PCB directly here: https://oshpark.com/shared_projects/IuYnoGB9

# Features

- Both Xbridge & Xdrip circuit support, selectable via a switch
- Battery can be soldered directly on the PCB or via a JST-2 connector
- Charging Status LED

# Components:

- 3x 1206 SMD Resitors (150Ω, 10kΩ, 27kΩ)
- 1x 1206 Red LED (any led should work)
- 2x 1206 SMD Capacitor 10μf
- 2x micro switch MSK-12C02
- 1x micro usb socket (ebay id: 121829362799)
- 1x MAX1811 lithium charger IC
- 1x JST-2 connector (optional)
- 1x HM-11 Bluetooth V4.0 Transceiver BLE Module (i got the one from fasttech)
- 1x Polulu Wixel
- 1x LiPo/Li-ion Battery

Attention! The MAX1811 Charger IC is set to 500mah. Only use a battery with more than 500mah.

# PCB Assembly

The components are large enough to be soldered by hand, the trickiest for me was the micro usb socket. If you use a hot air rework station (35$ on ebay) it should be easy.
![alt text](https://github.com/mzst123/Xdrip-Lipo-Board/blob/master/PCB%20Layout.png)


# Schematics

![alt text](https://github.com/mzst123/Xdrip-Lipo-Board/blob/master/Schematics.png)