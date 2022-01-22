# IRYamaha

I based this fork on aamarioneta/IRDenon as well as devjklein/yamaha-rx-v363-ir-codes (https://github.com/devjklein/yamaha-rx-v363-ir-codes) and used some of the home assistant yaml code of @aneisch. The esphome configuration allows for remote controlling a Yamaha RX-V863 (and probably other models) via Home Assistant through a jack 3.5mm plug in the "remote in" port of the receiver. I used a mono plug and connected it to ground and D2 connectors of a Wemos D1 mini ESP8266 board.

I used the following 3D print model as a case for the Wemos board:
https://www.thingiverse.com/thing:2847539/files

The codes on devjklein's repo are confirmed to work with the RX-V363, most also work with the RX-V863. I defined a number of services in my yaml file, in addition it is possible to apply other codes through a generic service call in Home Assistant developer tools. 

ESPHome: esp_yamaha_remote_1code or ESPHome: esp_yamaha_remote_2code

For a complete overview of codes refer to:

https://github.com/ronaldt80/IR-Yamaha-RX-V863/blob/master/Extended_IR_Codes_RX-V685RX-A780-RX-A3080CX-A5200_6.pdf

In the examples I included my card in home assistant which allows me to use the basic controls:

![image](https://user-images.githubusercontent.com/53364332/150644061-5adbca07-7db1-4e25-93f3-7bfdd5bd3a7a.png)
