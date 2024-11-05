Firmware is released as 2 different HEX having only the config word set in a different manner:  
  
-xtal.hex : is made for the PIC16F15376 having an external crystal oscillator on OSC1 and OSC2 pins (13 and 14). Crystal must be 8MHz. 4xPLL is used so the FOSC is 32MHz  

-intosc.hex : is made for using the PIC16F15376 without the external oscillator, so it's good also for the PIC16F15376 Curiosity Nano. It uses the HFINTOSC with 2x PLL and HFINTOSC set to 16MHz, so the FOSC is always 32MHz

Version		Release date	Description
1.00		23-10-2024		First release
1.00b		05-11-2024		LVP flag is ON in the config word: can be programmed with MPLAB SNAP   