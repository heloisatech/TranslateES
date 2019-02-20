# Localized EmulationStation

This is a localized fork of [Retropie's EmulationStation fork](https://github.com/RetroPie/EmulationStation).

Inspired by similar work on the Recalbox fork.

***

## Languages currently supported 

* Portuguese (Brazilian)
* Spanish
* French
* Italian
* Japanese
* Catalan

***

## How to use the localized EmulationStation

### **1.** Resolve Dependencies Of Libraries

`sudo apt-get install -y libboost-system-dev libboost-filesystem-dev libboost-date-time-dev libboost-locale-dev libfreeimage-dev libfreetype6-dev libeigen3-dev libcurl4-openssl-dev libasound2-dev cmake libsdl2-dev`

***

### **2.** Create a Clone from GitHub

`cd /home/pi/`

`git clone --recursive https://github.com/flyinghead/EmulationStation.git`

***

### **3.** Copy the Locale Directory

`copy -r locale/lang/fr locale/lang/(Your locale)`

***
 
### **4.** Compile EmulationStation

`cd EmulationStation`

`mkdir build`

`cd build`

`cmake ..`

`make`

***
  
### **5.** Test Run EmulationStation
_Be aware that your system must be set to the same locale that you want EmulationStation to run on._

`cd EmulationStation`

`LANG=(Your locale).UTF8 ./emulationstation`

 ***

### **6.** Install Emulationstation

`cd EmulationStation`

`sudo cp ./emulationstation /opt/retropie/supplementary/emulationstation/`

`sudo cp -r locale /opt/retropie/supplementary/emulationstation/`

***

## Author

[Flyinghead](https://github.com/flyinghead)

***

## Credits

Portuguese (Brazilian) and Spanish translations [heloisa](https://github.com/heloisatech)

_Thanks to:_

* [hiulit](https://github.com/hiulit) - For the Catalan translations
* [wakaya](https://retropie.org.uk/forum/user/wakaya) - For the Japanese translations
* Unknown - For the Italian translations
* [flyinghead](https://github.com/flyinghead) - For the French translations

* [wakaya](https://retropie.org.uk/forum/user/wakaya) - For the Installation tutorial
