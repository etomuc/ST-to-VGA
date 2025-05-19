# ST-to-VGA - a cheap and simple adapter to connect your ST to a (15.6kHz compatible) VGA monitor

ST-to-VGA is an adapter to connect a VGA monitor to an Atari ST and switch between colour and monochrome modes. The VGA monitor needs to support a vertical frequency of 15.6kHz. 
A list of supported monitors can be found here: [http://15khz.wikidot.com/](https://15khz.miraheze.org)

The design is basically the same that has been used in the 80s to connect the ST to a multisync monitor: https://mikrosk.github.io/doitarchive/doit_st/120902.htm

plus 2 capacitors which can improve image quality as explained here (German): https://www.chzsoft.de/site/hardware/diverse-kleinigkeiten-fur-den-atari-st/#adapter-monitorausgang-atari-st-nach-vga-nur-monochrom

The PCB is designed so it (hopefully) fits all ST models incl. the Mega ST.

## The components

<img src="/pictures/components.jpg" width="400"/>

1. PCB - order e.g. from JLCPCB
2. VGA connector female (*)
3. 3.5mm audio plug mono (female)
4. 13pin DIN - ST monitor connector (male)
5. 4P2T slide switch - 12pin 2 position
6. 3x resistor 75Ohm 
    1. depending on ST model and monitor, the best value can be somewhere between 0 and 100 Ohms
    2. optional: variable resistor
7. 3D printed spacer for monitor plug (optional)
8. capacitor 10nF (optional)
9. capacitor 470pF (optional)

<sup>(*) the PCB has been designed so that normal plugs as used in connector cables can be used. Panel mount connectors would probably have been the "better" solution but I wasn't aware of those when I designed the PCB.</sup> 

## Building the adapter

Solder all components except for the monitor connector from the upper side of the PCB. Take special care with the VGA connector as there is very little spacing between the through-holes and using e.g. excessive soldering paste can lead to shorts.

<img src="/pictures/1.jpg" width="250"/>

<sub>option: with variable resistors</sub><br/>
<img src="/pictures/1a.jpg" width="250"/>

Solder the monitor connector from the other side. You can add a 3D printed spacer to gain 1 or 2 mm distance from the STs case. This is optional but can be helpful if the adapter is later put into a 3D printed case. 

<img src="/pictures/2.jpg" width="250"/> <img src="/pictures/3.jpg" width="250"/> <img src="/pictures/5.jpg" width="250"/>

Make sure to keep the pins on this side as short as possible, especially if you want to put it into the 3D case:
<img src="/pictures/4.jpg" width="250"/>

## 3D printed case

<sub>optional support for connector screws:</sub><br/>
<img src="/pictures/case1.jpg" width="400"/>


<img src="/pictures/case2.jpg" width="250"/>

<sub>without and with hole to access variable resistors:</sub><br/>
<img src="/pictures/case3.jpg" width="400"/>
