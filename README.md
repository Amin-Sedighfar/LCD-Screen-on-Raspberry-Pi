# LCD-Screen-on-Raspberry-Pi
Download both files, put them into the same folder, then run the script.
And here is the network diagram of the way each pin should be connected.
![Untitled11](https://user-images.githubusercontent.com/87240174/223600446-5e47c1a8-2354-4943-9f37-d24e3b1e9cdc.jpg)
PINs information:
VSS (Ground): Connect this pin to GND on the Raspberry Pi.

VDD (Power): Connect this pin to the 5V pin on the Raspberry Pi.

V0 (Contrast): Connect this pin to a 1k Ohm resistor and then to the ground. In case of using a potentiometer to adjust the contrast: A potentiometer has 3 pins, connect the centre pin of the potentiometer to V0 of the LCD, one pin to the ground, the last one is not used.

A (Brightness): Connect this pin to a 10 Ohm resistor and then to the ground. In case of using a potentiometer to adjust the brightness: A potentiometer has 3 pins, connect the centre pin of the potentiometer to VCC (power), one pin to A, the last one is not used.

RS (Register Select): This pin determines whether the data sent to the LCD screen is a command or a character. Connect this pin to GPIO 26 on the RaspberryPi.

RW (Read/Write): This pin determines whether the data sent to the LCD screen is a read or a write operation. Connect this pin to GND on the Raspberry Pi.

EN (Enable): This pin enables the LCD screen to read the data on its data pins. Connect this pin to SP11 MISO on the Raspberry Pi.

D4: GPIO 13

D5: GPIO 6

D6: GPIO 5

D7: SP10 SCLK
