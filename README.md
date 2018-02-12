# Italian keyboard layout for Digispark DigiKeyboard
Original files: https://github.com/digistump/DigistumpArduino/tree/master/digistump-avr/libraries/DigisparkKeyboard

The two header files must be put into the DigisparkKeyboard library in your Arduino15 folder.


Windows (Arduino IDE 1.6.5 and previous):
```
c:\Users\(username)\AppData\Roaming\Arduino15\packages\digistump\hardware\avr\(version)\libraries\DigisparkKeyboard\
```
Windows (Arduino IDE 1.6.6 and later):
```
c:\Users\(username)\AppData\Local\Arduino15\packages\digistump\hardware\avr\(version)\libraries\DigisparkKeyboard\
```
Linux:
```
/home/(username)/.arduino15/packages/digistump/hardware/avr/(version)/libraries/DigisparkKeyboard/
```
---
In order to be able to send \[]{}@#, I modified the write function in DigiKeyboard.h on line 203 to send the corresponding keystroke combinations.

scancode-ascii-table.h have been updated to send the correct keycode given an ASCII code.

---

Useful links: 
- https://github.com/PaulStoffregen/cores/blob/master/teensy/keylayouts.h
- http://www.asciitable.com/
