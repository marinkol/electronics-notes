Arduino Nano Clones
===================

Source from Ebay:
[Makershop][1]



You can buy them [soldered][1] or [NOT soldered][2]
This boards have different USB chipsets (CH340), than original, and require special drivers to be installed.

Drivers can be found in drivers subfolder, or [arduino eu][4] site.

Driver details:

    CH340, CH340G & CH341 (USB-SERIAL chip) V3.4
    Driver Version = 08/08/2014, 3.4.2014.08

Install through Windows Device Manager

Configure test system
---------------------

Either install [Arduino software][5], or use their [cloud offerning][6], Install the above driver
and then start the arduino studio.

Select `Board -> Arduino Nano` and processor `ATMEGA328P (Old Bootloader)`.
Connect arduino to usb, and now you should see tools port option, select your board.



Run hello world
----------------

Under `File` `Examples` `Built-in Examples` `01. Basics` select `Blink`
Compile and upload.
If everything is ok, orange light should be blinking.

Trubleshooting:
If you see
```
    avrdude: stk500_getsync() attempt 1 of 10: not in sync: resp=0x00
```
That means arduino can't comunicate with board correctly so you need to recheck your setup.



[1]: https://www.ebay.de/str/sensusshop
[2]: https://www.ebay.de/itm/Arduino-Nano-Atmega328P-BEREITS-GELOTET-verlotet-fertig-aufgebaut/253638131454?hash=item3b0e02befe:g:2uMAAOSwrpJb4H0C
[3]: https://www.ebay.de/itm/Nano-V3-0-ATmega-328-Board-CH340-USB-Chip-Arduino-Kompatibel/252742123829?hash=item3ad89ac135:g:xCEAAOSwPGtb33e0
[4]: https://www.arduined.eu/ch340-windows-8-driver-download/
[5]: https://www.arduino.cc/en/Main/Software
[6]: https://create.arduino.cc/