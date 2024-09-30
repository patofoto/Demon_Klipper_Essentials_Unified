
If you feel these macros are valuable enough to download & use please consider hitting that "sponsor this project" button or the Ko-Fi image below or at https://ko-fi.com/3dprintdemon & buying me a beer/coffee. Its always very much appreciated & anything you do send goes towards helping me continue putting my ideas out there for the whole 3D printing community. Sending even a little makes a difference! Thank you & happy printing!!

[<img width="171" alt="kofi_s_tag_dark" src="https://github.com/3DPrintDemon/Demon_Klipper_Essentials_Unified/assets/122202359/08473899-563b-4b4d-9409-5e6602d6ec44">](https://ko-fi.com/3dprintdemon)

****************************************************************************************************************************
### IF YOU RAN V1.0-V2.8 BE SURE TO UPDATE YOUR SLICER'S START GCODE OR NEW FEATURES WONT WORK!
**Also you must update ALL the macro files as this new version will NOT work correctly with old files!**
****************************************************************************************************************************



# IF YOU'RE USING A SOVOL SV08 PRINTER! 

BE SURE TO INSTALL THE STUFF YOU NEED TO INSTALL!!!

- https://github.com/3DPrintDemon/KAMP_LiTE/releases/tag/v1.0
- https://github.com/3DPrintDemon/Voron-Stealthburner/blob/main/Firmware/RGB_LEDs.cfg
- https://github.com/3DPrintDemon/Non_Blocking_Wait/releases/tag/Heat_Soak_Timers_V1.0
  
###### Note: These files are requred for the macro pack to work correctly. Install even if you dont have any LEDs & set a dummy pin.

Here is my SV08 nozzle cleaning & purge bucket!

- https://www.printables.com/model/873006-sovol-sv08-silicone-nozzle-cleaner-purge-bucket-mi

Anti-vibration feet

- https://www.printables.com/model/867321-sovol-sv08-low-profile-vibration-isolation-feet

M12 Probe mount

- https://www.printables.com/model/870302-sovol-sv08-m12-inductive-probe-mount-lj12a3-4-zax

DIN rail mount

 - https://www.printables.com/model/867676-sovol-sv08-recessed-din-rail-mount-bracket

****************************************************************************************************************************

# Edit your printer.cfg 

Be sure your `printer.cfg` file `[extruder]` section contains...

```
max_extrude_only_velocity: 15
```
This is used by the load/unload macros & is converted into feedrate of mm/s & is limited to 20

```
[idle_timeout]
gcode:
    _DEMON_IDLE_TIMEOUT
timeout: 3600
```

This will call the new Demon timeout macro after 1 hour & execute the functions of your choice in the demon_user_settings file. You csan set the time (seconds) to anything you like.


YOU MUST, I REPEAT MUST DISABLE ALL THE SOVOL MACROS BY COMMENTING OUT THE macro.cfg FILE INCLUDE IN THE printer.cfg FILE! 
To do this use a # at the start of the line like this:
```
# [include Macro.cfg]
```
Then set your fans like this in the printer.cfg file:
```
[multi_pin fan_pins]
pins: extra_mcu:PA7, extra_mcu:PB1

[fan]
pin:multi_pin: fan_pins
max_power: 1.0
```
Comment out the stock entry do not delete it, it must look like this:
```
# [fan_generic fan0] # back model cooling fan
# pin: extra_mcu:PA7
# max_power: 1.0

# [fan_generic fan1] # front model cooling fan
# pin: extra_mcu:PB1
# max_power: 1.0
```


****************************************************************************************************************************





I hope this macro pack makes a nice difference to your printing life, don't forget, if you feel its valuable enough to use please consider hitting that "sponsor this project" button & buying me a beer/coffee. Its always very much appreciated. Thank you & happy printing!!

[<img width="171" alt="kofi_s_tag_dark" src="https://github.com/3DPrintDemon/Demon_Klipper_Essentials_Unified/assets/122202359/08473899-563b-4b4d-9409-5e6602d6ec44">](https://ko-fi.com/3dprintdemon)
