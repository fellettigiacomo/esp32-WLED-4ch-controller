# esp32-WLED-4ch-controller
Hardware design for a 4 channel WLED controller with built in relays for power saving and level shifter for better signal integrity with long data cables.<br>
<br>![alt text](https://github.com/fellettigiacomo/esp32-WLED-4ch-controller/blob/main/board-render.png?raw=true)

## Manufacturing
I tried to make this board as cheap as possibile using JLCPCB basics part for PCBA, however, since there are many extended parts the final cost should be around 25$/board + shipping
<br>All parts should be compatible with the JLCPCB assembly, otherwise, feel free to send me a pull request.
<br>Looking for a cheaper alternative? i've uploaded a version of the board without the esp32 related hardware, with the headers to plug a whole dev-kit, saving out on extended parts.

## Compatibility and capabilites
This PCB supports up to 4 addressable led strips:
Only strips that works with 5V are compatible. 
Compatible strips: WS2811 - WS2812B - TM1829 (and other with 5V, DATA, GND). Check [the wled wiki](https://kno.wled.ge/basics/compatible-led-strips/) for more info
The board allows for a maximum current of around 100W (20A) max. Maximum current for a single relay is 10A (50W)


## Flashing
To flash the firmware, follow these steps:
- connect via USB-C or with serial UART (use test points TX, RX, 3.3V, GND)
- use the WLED web installer powered by Esp Web Tools at https://install.wled.me/
- connect to serial port and flash
- after installing, connect to the address provided from the web installer, or connect to the WLED AP
- done! enjoy your addressable IoT leds :D

## Licence
CERN Open Hardware License - S (CERN-OHL-S)
