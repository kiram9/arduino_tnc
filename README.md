arduino_tnc
===========

Arduino esque Soft TNC for Packet Radio (1200 baud)


    Arduino TNC
    
    This is a TNC based on Arduino hardware, intended primarily for APRS.
    Wherever possible, low-level AVR registers are used instead of the high-level Wiring
    libraries, in order to minimize the program size and maximize performance. This code
    is experimental, buggy, and is probably not suitable for any purpose. That said, it 
    is also small, fast, heavily commented, and might even decode a packet occasionally.

    This software is based heavily on the (far better) works of:
    
      Bob Bruninga, WB4APR
      Dennis Seguine
      Scott Miller, N1VG
      Gary Dion, N4TXI
      John Hansen, W2FS
      Thomas Sailer, HB9JNX/AE4WA
      
    Anyone wanting to use this code is strongly encouraged to:
    
      1. Reconsider.
      2. Buy a pre-made device from "argentdata.com" or "tncx.com" instead.
      3. At the very least, download the datasheet for the ATmega328P and/or ATmega1280.
      4. Bookmark "http://www.nongnu.org/avr-libc/".
    
    If you do find anything useful about this code, please let me know, at:
   
    Kilo India Four Mike Charlie Whiskey at-sign Golf Mike Alpha India Lima Dot Com.
    
    
    Robert Marshall, KI4MCW    
    
    
    Transmit code based on  Whereavr http://www.garydion.com/projects/whereavr/
    added by Kieran Levin, KC9BZY kieranlevin.com kilo india ralf alpha Mike 9 at-sign yahoo dot com
    to use with programming over bluetooth I prefer the ladyada no wait booloader 
    http://www.ladyada.net/library/arduino/bootloader.html
    you can just set the serial port and arduino board to BT, hit reset on the board
    and then press program to use over bluetooth with a OEMSPA310 connectblue BT-serial 
    adapter 
    hardware for tranmist is copied from whereavr 
    
    
    Version history:
20100602 (0.14) Kiss transmit added, increased buffer size changed uart speed to 19200 to match arduino bootloader, changed heartbeat off, ADCREF is set to VCC, DISCONNECT AREF from power supply to prevent damage to chip and only connect external cap ~0.1uF
20100409 (0.13) Auto-bias, KISS output.
20100408 (0.12) Switch to Seguine math, handle Due vs Mega hardware thru config options.
20100401 (0.06) Last attempt with Fourier math.
20100323 (0.01) First draft.
    
