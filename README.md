# Open-T12-Soldering-Station-
This is a clone of the cheap(KSGER) T12 soldering stations, attempting to eliminate the shortfalls of cheap.  Useless without the fine firmware from https://github.com/deividAlfa/stm32_soldering_iron_controller

It has provisions for a backup battery. Jumper selectable between internal and external NTC as some of the new handles don't contain a NTC, so this gives you the option if you don't want to add one.  There are also jumper option for configuring diffrent soldering handles.  It is setup to use the KSGER 1.3 OLED 6 pin display.  More specifics if you want to fin your own display.

The design STM32 pinouts match the later KSGER stations for compatibility with the above mentioned firmare. There is no provision for the realtime clock in the firmware, yet it might still be functional, I see it as useless.

Some of the cheap boards had issue with the linear voltage regulator dropping out from thermal protection as the power was quite high dropping from 24V to 3.3V.  This design uses a switching regulator to step down from 24V ot 5V, and then a 3.3V regulator for a clean 3.3V supply.

Much more information on the many models out there at the above mentioned site for the firmware. I created this as it is impossible to tell exactly what you are buying from the suppliers.

![Alt text](pictures/Front.png?raw=true "Front")

![Alt text](pictures/Rear.png?raw=true "PCB")

![Alt text](pictures/PCBlayout.png?raw=true "PCB Layout")

![Alt text](pictures/schematic.png?raw=true "Schematic")

A limited run will be available soon on Tindie.
