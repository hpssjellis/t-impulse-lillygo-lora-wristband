# t-impulse-lillygo-lora-wristband


Good setup by @Roshankattel

https://brief-tadpole-2d3.notion.site/TTGO-T-Impulse-49f8f052f09641499c563194c666f813



.

.


Main github  https://github.com/Xinyuan-LilyGO/T-Impulse

Downloading this github has some folders that may help with the install on Arduino. The main install is setup for Platformio.org which might be a good route.

So far I can see the DFU connection but can't install a program. On platformio the S76G-Factory code compiles but does not load.

[S76G-Factory](https://github.com/Xinyuan-LilyGO/T-Impulse/tree/master/Example/S76G-Factory)

possible incorrect arduino IDE json link

This link has a json that works

https://github.com/stm32duino/Arduino_Core_STM32

The json for the arduino IDE is Note: ```main```` instead of ```master```

https://github.com/stm32duino/BoardManagerFiles/raw/main/package_stmicroelectronics_index.json


## First steps Oct26, 2023

USB-C cable issue. It has to be pushed all the way in. not really obvious

Check windows device manager both the com-ports and the Universal serial bus controllers
In the com ports it might show both the regular serial port and the STM32-bootloader  the Universal serial port only shows the ST loader showing up on some windows computers. I am using win11

Get used to how to put the t-impulse into serial and DFU modes using the buttons.

boot nearest usb-c connecto  
reset farthest away from usb-C serial port

1. reset resets the t-impulse takes about 3 seconds to load.
2. boot then prog-in usb-C and get into DFU-mode   OR   boot and reset, then release reset then 2 seconds later release reset, then release boot works but get used to it.
3. 

This link may have some drivers

This link may be useful   https://www.onetransistor.eu/2017/11/stm32-bluepill-arduino-ide.html




This might be useful
https://github.com/stm32duino/Arduino_Core_STM32/wiki/Upload-methods#stm32cubeprogrammer




## Useful Info

Board Number ```nucleo_l073rz```


Images here are super useful

https://github.com/Xinyuan-LilyGO/T-Impulse/tree/master/image

The DFU- util is what is needed for installing windows but use the above images to figure out how to do it.

I did not have a driver installed so my image is slightly different. When it finished it looked like this


<img width="429" alt="image" src="https://github.com/hpssjellis/t-impulse-lillygo-lora-wristband/assets/5605614/73b76abc-f2c7-4b4e-92a4-8933079d54cd">





