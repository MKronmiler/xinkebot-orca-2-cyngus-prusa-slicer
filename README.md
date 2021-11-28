# xinkebot-orca-2-cyngus-prusa-slicer
This project contains a Prusa Slicer config bundle for the Xinkebot Orca 2 Cygnus

I was given this printer as a gift and discovered how much of a clusterf*&k it is.

I've made a config bundle for people to use if they also have this printer in the **SINGLE Extruder** configuration

If someone has a dual extruder model that has time to help work on a profile please email me at michael@kronmiller.dev

# Config Bundle Overview

The config bundle is a work in progress **these are my settings and will likely require some adjustments as I spend more time printing.** I strongly encourage anyone to fork this and make adjustments to settings as they work with thier printer.

Printer Profile with proper sized build volume and extruder settings

## Printing Settings
1. 0.15mm detail print settings for a 0.4mm nozzle 

## Filament Settings
1. PLA Profile
2. PETG Profile

For whatever reason this printer does not use traditional M codes for heating the nozzle. I went through their example prints and found what I believe to the the correct M codes. This should be included in the custom g-code in the config bundle but in the event it isn't here is a breakdown of the code.

Check the media folder to find where in Prusa Slicer you can find it

### Special Printer Settings

```
;Custom End G-Code
;Custom Code Changes
M140 S0 ; turn off bed
M104 S0 T0 ; turn off extruder
```

### Special Filament Settings

```
; Filament gcode
M82
M106 S0
M140 S60 ; bed set temp?
M190 S60 ; wait for bed temp?
M104 S235 T0 ; extruder temp?
M109 S235 T0 ; wait for extruder temp?
```

# Octoprint Functionality

The Xinterbot Orca 2 Cygnus is one of the lucky few printers to ship from the factory with broken firmware. If you plan on using octoprint then you will need to install [Fix CBD Firmware](https://plugins.octoprint.org/plugins/fixcbdfirmware/)

# Additional Inclusions
 As a result of Xinterbot nuking thier website, most of the support files are completely inaccesible. I have included a [Google Drive Folder](https://drive.google.com/drive/folders/1lf32KrpIDn3X5aE5yBrrZYkoU7oYfOv3?usp=sharing) with all the included files this printer came with on the SD card.

 This includes test prints, video tutorials, and setup files for the Orca 2 Cygnus
