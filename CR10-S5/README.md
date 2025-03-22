# CR-10 S5 Configuration files

This file is specific to my printer and mods.  You will need to update it if your configuration is not the same as mine

- BTT SKR Mini E3 v3.0 control board
- Aftermarket 500x500 bed heater (heater NOT connected to main board)
- BTT SFS V2.0 Smart Filament Sensor
- Genuine ANTCLabs BLTouch probe


################   WARNING ######################
** 'Important wiring notes' **

The BLTouch wiring instructions from BTT are WRONG.
Properly wiring the BLTouch will require installing new crimped ends (JST & Dupont respectively) on the BLTouch wires

See the picture at https://imgur.com/a/8XDG1ay

The instructions call for all five pins (or four in some cases of stock Creality CRTouch) to be connected to the IO port.  This is the connector to the left of the red jumper at the bottom of the picture from the link above.   THIS IS WRONG

Instead, one ground wire, and the sense wire, should be connected to the "Z Endstop" connector on the board.  The "pin control" wire, +5v, and secondary ground wire (if present) still get connected to the three left most pins on the IO port.
