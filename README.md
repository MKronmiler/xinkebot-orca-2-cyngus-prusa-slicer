# xinkebot-orca-2-cyngus-prusa-slicer
This project contains a Prusa Slicer config bundle for the Xinkebot Orca 2 Cygnus

I was given this printer as a gift and discovered how much of a clusterf*&k it is.

I've made a config bundle for people to use if they also have this printer

# Config Bundle Overview

The config bundle is a work in progress **these are my settings and will likely require some adjustments as I spend more time printing.** I strongly encourage anyone to fork this and make adjustments to settings as they work with thier printer. 

Printer Profile with proper sized build volume and extruder settings

## Printing Settings
1. 0.15mm detail print settings for a 0.4mm nozzle 

## Filament Settings
1. PLA Profile
2. PETG Profile

### Special Filament Settings

For whatever reason this printer does not use traditional M codes for heating the nozzle. I went through their example prints and found what I believe to the the correct M codes. This should be included in the custom g-code in the config bundle but in the event it isn't here is a breakdown of the code.

```
; Filament gcode

M82

M106 S0

M140 S60 ; bed set temp?

M190 S60 ; also probably bet set temp???

M104 S225 T0 ; nozzle temp???

M109 S225 T0 ; nozzel temp also????? 

```

# Octoprint Functionality

# Additional Inclusions
]
