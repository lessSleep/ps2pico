# ps2pico
USB keyboard to PS/2 interface converter using a Raspberry Pi Pico

Connect a USB keyboard using an OTG-adapter and PS/2 5V to Pico VBUS.

3.3V to 5V conversion is done with two NPN transistors as shown below:
```
                   PS/2 CLOCK
                       |
            ____       |
GPIO 15 ___|2k2 |____|/   BC547
           |____|    |\e
                       |
                  _____|__GND


                   PS/2 DATA
                       |
            ____       |
GPIO 16 ___|2k2 |____|/   BC547
           |____|    |\e
                       |
                  _____|__GND
```

WORK-IN-PROGRESS
(final version will be written in Rust https://github.com/No0ne/ps2pico-rs)