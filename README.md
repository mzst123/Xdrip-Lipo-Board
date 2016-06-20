# Xdrip Lipo Bluetooth Board PCB
Xdrip on a printed circuit board!

The design files are in the folder ["Eagle PCB Files"](https://github.com/mzst123/Xdrip-Lipo-Board/tree/master/Eagle%20PCB%20Files)

Or you can order the PCB directly [here](https://oshpark.com/shared_projects/IuYnoGB9)

For other versions of this project check out the folder ["Other Versions"](https://github.com/mzst123/Xdrip-Lipo-Board/tree/master/Other%20Versions)

If you can't solder this board and need help send me an email and im sure we can figure something out. My e-mail address is my github username at gmail.com

## Features:

- The board uses a MAX1811 battery charging ic
- Both Xbridge & Xdrip circuit support, selectable via a switch
- Battery can be soldered directly on the PCB (2.54mm header) or via a JST-2 connector (2mm pitch)
- Charging Status LED (On = charging; off = full)

## Components:

- 3x 1206 SMD Resitors (150Ω, 10kΩ, 27kΩ)
- 2x 1206 SMD Capacitor 10μf
- 2x micro switch MSK-12C02
- 1x 1206 Red LED (any led should work)
- 1x micro usb socket (ebay id: 121829362799)
- 1x MAX1811 lithium charger IC
- 1x [JST-2 connector 2mm pitch](https://www.sparkfun.com/products/8612) (optional - your battery needs to have the mating connector - sparkfun sells compatible batteries, or buy the connector separately and crimp it on your battery)
- 1x HM-11 Bluetooth V4.0 Transceiver BLE Module (I got the one from fasttech)
- 1x Polulu Wixel
- 1x LiPo/Li-ion Battery (I recommend using a LiPo battery)

Attention! The MAX1811 Charger IC is set to 500mah. Only use a battery with more than 500mah.

I source most of my components from eBay because of the free shipping. Here are some example links but consider that the prices change daily and shipping depends on where you are located:
- [Resistors](http://www.ebay.com/itm/100pcs-1-4W-watt-1206-SMT-SMD-Chip-Resistor-from-0-ohm-to-10M-ohm-1-/252380762812?var=&hash=item3ac310d2bc:m:msXv_-i2Opl1RPDANdY3cMw)
- [Capacitors](http://www.ebay.com/itm/12pcs-1206-smd-tantalum-capacitor-16v-10uf-106-10-3216-a-type-ic-diy-develop-d1-/331840663464?hash=item4d433eafa8:g:MpYAAOSwubRXFXfc)
- [Micro Switch](http://www.ebay.com/itm/20-pcs-MSK-12C02-Mini-SPDT-1P2T-Slide-Switch-On-Off-SMD-7-Pin-For-MP3-MP4-/161857451517?hash=item25af74b5fd:g:e1IAAOSwl9BWHbT4)
- [Red Led](http://www.ebay.com/itm/10-x-1206-RED-Super-Bright-LED-Chip-SMD-SMT-Bulb-Lamp-Light-High-Brightness-RoHs-/191231419928?hash=item2c8647e618:g:O3sAAOSw9N1Vo3OF&vxp=mtr)
- [micro usb socket](http://www.ebay.com/itm/2015-New-10Pcs-Micro-USB-B-Female-5Pin-SMT-Socket-Connector-Hot-Sale-MO-/401091696043?hash=item5d62ed95ab:g:R2kAAOSwDNdVpfv5)
- [Max1811](http://www.ebay.com/itm/1PCS-USB-LI-CHARGER-IC-MAXIM-SOP-8-MAX1811ESA-MAX1811ESA-MAX1811ESA-T-/272041007390?hash=item3f56e8591e:g:rx0AAOSwAYtWPgb~)
- [LiPo battery](http://www.ebay.com/itm/3-7V-850mAh-Lipo-Polymer-li-ion-Battery-703040-for-cell-phone-Camera-DVD-GPS-PAD-/111909510772?hash=item1a0e539e74:g:FAoAAOSwFNZWxojb)
- [Bluetooth module(Fasttech)](https://www.fasttech.com/product/1740900-hm-11-bluetooth-v4-0-transceiver-ble-module)


## PCB Assembly:

Everything is labeled on the PCB. The components are large enough to be soldered by hand, the trickiest for me was the micro usb socket. But if you use a hot air rework station (40$ on ebay) it should be very easy.

Here is a video how-to

<a href="http://www.youtube.com/watch?feature=player_embedded&v=SYGwYvehjtA
" target="_blank"><img src="http://img.youtube.com/vi/SYGwYvehjtA/0.jpg" 
alt="IMAGE ALT TEXT HERE" width="240" height="180" border="10" /></a>

[![IMAGE ALT TEXT HERE](http://img.youtube.com/vi/SYGwYvehjtA/0.jpg)](http://www.youtube.com/watch?v=SYGwYvehjtA)

![alt text](https://github.com/mzst123/Xdrip-Lipo-Board/blob/master/Images/PCB%20Layout.png)


## Schematics:

![Schematics](https://github.com/mzst123/Xdrip-Lipo-Board/blob/master/Images/Schematics.png)

## Software:
For the Wixel software i recommend [xBridge](https://github.com/jstevensog/wixel-sdk/tree/master/apps/xBridge2) from [John] (https://github.com/jstevensog). Just download the .wxl file and load it to the wixel. There are many advantages of xBridge, for example you don't have to re-compile the program to change transmitters because you can set it inside the xDrip app, improoved power saving features, battery level estimate, etc...

[Here](https://github.com/StephenBlackWasAlreadyTaken/xDrip/wiki/xdrip-beta) you can download the latest xDrip android app.

## 3D Enclosure:

I made an enclosure, however it has not been tested yet. To further reduce space, the JST-2 connector is not used in this design. In the future I might add one with JST-2 support. The battery compartment should fit an 850mah Lipo Battery. The .STL files are int the "Enclosure" Folder.
![Enclosure](https://github.com/mzst123/Xdrip-Lipo-Board/blob/master/Images/3D_render.png)

## Pictures:

![Top View](https://github.com/mzst123/Xdrip-Lipo-Board/blob/master/Images/Top.JPG)
![Bottom View](https://github.com/mzst123/Xdrip-Lipo-Board/blob/master/Images/Bottom.JPG)
![Side View](https://github.com/mzst123/Xdrip-Lipo-Board/blob/master/Images/Side.JPG)
![Screenshot](https://github.com/mzst123/Xdrip-Lipo-Board/blob/master/Images/Screenshot.png)