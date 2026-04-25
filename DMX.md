DMX (Digital MultipleX) is a digital lighting standard.

On the light you assign:
* An address from 1-512
* the amount of addresses to assign.
This then becomes the address block for the light so:
If a lights address 1 and has 4 channels it will use channels 1,2,3,4
If a lights address is 12 and has 4 channels it will use channels 12,13,14,15
If a light has address 112 and has 8 channels it will use channels 112,113,114,115,116,117,118,119

Each light model has a different standard configuration. 
The [[Plano_Spot_7TC]] for example only has a 4 channel mode. 
Those channels are:
1. Red
2. Green
3. Blue
4. Channel mode:
	1. dimmer/sound/strobe
	2. Dimmer 
	3. Dimmer/sound
	4. Dimmer/Sound/color macro

If the Light is set to address 1 and we use channel mode 2 addresses are:
1. Red
2. Green 
3. Blue
4. Dimmer

if the light is set to address 12 and we use channel mode 2 addresses are:
12. Red
13. Green
14. Blue
15. Dimmer
For most lights if there is a dimmer the color and the dimmer both have to be set so to have a red light both Red and Dimmer have to be on.


Lights are unaware of each other. Most of the time we want to avoid this.
If I have Two [[Plano_Spot_7TC]] lights set:
Light 1 starting on channel 1
Light 2 starting on channel 3
If I turn on channel 3,4 and 6
Light 1 will have a blue light on 
Light 2 will have a Red and Green light on.

