Digistump alternative
=====================

Bought from:
[Maker de][1]

Original from:
[Digistump][2]

It's _Arduino_ based on ATinny 85

Instalation
-----------

Go to [Digistump wiki][3] and follow the procedure there.
In new Arduino IDE's installers errors out, so you need to manualy run
driver instalation (error message is helpfull too)

    

You can also find latest releases and drivers at [digisparks github][4] page.
[Latest Drivers][5]

Digistump uses [micronucleus][6] as their bootloader.


Test that it works
------------------

After driver instalation, inser digispark into usb slot,  
`Devices and Printers` should detect it as `Digispark Bootloader`

In Arduino select Board as `Digispark (Default 16.5 mhz)`
and upload the following code:

```c
// the setup routine runs once when you press reset:
void setup() {                
  // initialize the digital pin as an output.
  pinMode(0, OUTPUT); //LED on Model B
  pinMode(1, OUTPUT); //LED on Model A   
}

// the loop routine runs over and over again forever:
void loop() {
  digitalWrite(0, HIGH);   // turn the LED on (HIGH is the voltage level)
  digitalWrite(1, HIGH);
  delay(500);               // wait for a second
  digitalWrite(0, LOW);    // turn the LED off by making the voltage LOW
  digitalWrite(1, LOW); 
  delay(500);               // wait for a second
}
```

Further info [Digispark basics][7] and [Digispark wiki][8]

[1]: https://www.ebay.de/itm/Digispark-Mini-Arduino-USB-IDE-Attiny85-Kickstarter-Board-Modul/252735445592?hash=item3ad834da58:g:rjgAAOSwJJVb5Hyi
[2]: http://digistump.com/
[3]: https://digistump.com/wiki/digispark/tutorials/connecting
[4]: https://github.com/digistump/
[5]: https://github.com/digistump/DigistumpArduino/releases/download/1.6.7/Digistump.Drivers.zip
[6]: https://github.com/micronucleus/micronucleus
[7]: https://digistump.com/wiki/digispark/tutorials/basics
[8]: https://digistump.com/wiki/digispark/
