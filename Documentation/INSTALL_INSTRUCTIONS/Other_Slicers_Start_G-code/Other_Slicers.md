
If you feel these macros are valuable enough to download & use please consider hitting that "sponsor this project" button or the Ko-Fi image below or at https://ko-fi.com/3dprintdemon & buying me a beer/coffee. Its always very much appreciated & anything you do send goes towards helping me continue putting my ideas out there for the whole 3D printing community. Sending even a little makes a difference! Thank you & happy printing!!

[<img width="171" alt="kofi_s_tag_dark" src="https://github.com/3DPrintDemon/Demon_Klipper_Essentials_Unified/assets/122202359/08473899-563b-4b4d-9409-5e6602d6ec44">](https://ko-fi.com/3dprintdemon)

# ADD THE 3 LINES BELOW TO PRUSA SLICER'S START GCODE SECTION
```
M104 S0
M140 S0
PRINT_START EXTRUDER=[first_layer_temperature[initial_extruder]] BED=[first_layer_bed_temperature] LAYER=[layer_height] FILAMENT=[filament_type]
```


# IF YOU USE CURA ADD THE 3 LINES BELOW TO CURA SLICER'S START GCODE SECTION
```
M109 S0
M190 S0
PRINT_START EXTRUDER=\{material_print_temperature_layer_0\} BED=\{material_bed_temperature_layer_0\} LAYER=\{layer_height\} FILAMENT=\{material_type\}
```

# ADD THE 3 LINES BELOW TO SIMPLIFY3D SLICER'S START GCODE SECTION
This is untested, please notify if it doesnt work

```
M109 S0
M190 S0
PRINT_START EXTRUDER=[extruder0_temperature] BED=[platform0_temperature] LAYER=[current_layer_height] FILAMENT=[auto_configure_material]
```

# ALL SLICERS!!!


Also be sure to add the line below in your slicer's End G-Code box
```
PRINT_END
```

### Your slicer's Start G-Code box must only contain those 3 lines above, plus the Mainsail layer count command - see mainsail website, slicer.
### Your slicer's End G-Code box must only contain that line above
### https://docs.mainsail.xyz/overview/slicer


### These macros rely on you setting the correct filament type in your slicer! BE SURE YOU DO THIS! OR IT WILL NOT WORK!!
