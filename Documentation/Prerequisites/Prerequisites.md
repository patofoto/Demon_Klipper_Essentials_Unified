
If you feel these macros are valuable enough to download & use please consider hitting that "sponsor this project" button or the Ko-Fi image below or at https://ko-fi.com/3dprintdemon & buying me a beer/coffee. Its always very much appreciated & anything you do send goes towards helping me continue putting my ideas out there for the whole 3D printing community. Sending even a little makes a difference! Thank you & happy printing!!

[<img width="171" alt="kofi_s_tag_dark" src="https://github.com/3DPrintDemon/Demon_Klipper_Essentials_Unified/assets/122202359/08473899-563b-4b4d-9409-5e6602d6ec44">](https://ko-fi.com/3dprintdemon)

# Prerequisites

### Orca Slicer

Make sure you have the latest 2.2.0 (beta2) version of Orca Slicer DO NOT USE ORCA SLICER DOT NET!!! BAD!!!

This link GOOD!

- https://github.com/SoftFever/OrcaSlicer/releases

******************************

You must download & `[include]` these additional files along with these Demon Macros or they will NOT work correctly.


These additional macros are prerequisites:

### **FOR ALL MACHINES FOR ADAPTIVE PURGING & SMART PARK install KAMP_LiTE fork.**
- https://github.com/3DPrintDemon/KAMP_LiTE/releases/tag/v1.0

### **For VORON PRINTERS or other machines with toolhead Neopixels**
- https://github.com/VoronDesign/Voron-Stealthburner/blob/main/Firmware/stealthburner_leds.cfg
- https://github.com/3DPrintDemon/Non_Blocking_Wait/releases/tag/Heat_Soak_Timers_V1.0
  
###### Note: You will need to choose the "sb_leds" or "toolhead_leds" file versions. 

###### Note: This file is requred for the heat soaks to work correctly. Install even if you dont have any LEDs & set a dummy pin.

### **For SOVOL SV08 PRINTERS**
- https://github.com/3DPrintDemon/Voron-Stealthburner/blob/main/Firmware/RGB_LEDs.cfg
- https://github.com/3DPrintDemon/Non_Blocking_Wait/releases/tag/Heat_Soak_Timers_V1.0
  
###### Note: This file is requred for the heat soaks to work correctly. Install even if you dont have any LEDs & set a dummy pin.

### **For other machines without toolhead Neopixels**
- https://github.com/3DPrintDemon/Non_Blocking_Wait/releases/tag/Heat_Soak_Timers_V1.0
  
###### Note: This file is requred for the heat soaks to work correctly. Install even if you dont have any LEDs & set a dummy pin.

You must keep neopixels set to `False` in the `demon_user_settings_v2.9.cfg` `Hardware Options` section

******************************

- [Head on to General Setup For All Printers](https://github.com/3DPrintDemon/Demon_Klipper_Essentials_Unified/blob/main/Documentation/INSTALL_INSTRUCTIONS/General%20_Setup_For_All_Printers/INSTALL_INSTRUCTIONS.md)
