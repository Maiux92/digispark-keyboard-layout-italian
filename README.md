# Italian keyboard layout for Digispark DigiKeyboard
Original files: https://github.com/digistump/DigistumpArduino/tree/master/digistump-avr/libraries/DigisparkKeyboard

# Installation
You need to place the two header files `DigiKeyboard.h` and `scancode-ascii-table.h` into the **DigisparkKeyboard** library, inside your **Arduino15** folder.

### Windows (Arduino IDE 1.6.5 and previous):
```
c:\Users\(username)\AppData\Roaming\Arduino15\packages\digistump\hardware\avr\(version)\libraries\DigisparkKeyboard\
```
### Windows (Arduino IDE 1.6.6 and later):
```
c:\Users\(username)\AppData\Local\Arduino15\packages\digistump\hardware\avr\(version)\libraries\DigisparkKeyboard\
```
### Linux:
```
/home/(username)/.arduino15/packages/digistump/hardware/avr/(version)/libraries/DigisparkKeyboard/
```

# Info
For sending special characters, such as `\[]{}@#`, I modified the `DigiKeyboard.h` write function (line ~203), so to make it send the corresponding keystroke combination.

I also updated `scancode-ascii-table.h` so to map the correct keycodes to ASCII codes for the italian keyboard layout.

# References
I used these two resources: 
- https://github.com/PaulStoffregen/cores/blob/master/teensy/keylayouts.h
- http://www.asciitable.com/

# Other languages
- Spanish: https://github.com/Dasor/digispark-keyboard-layout-Spanish
- Portuguese: https://github.com/r4p3cks/digispark-keyboard-layout-portuguese
