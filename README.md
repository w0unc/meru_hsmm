# meru_hsmm
We have a bunch of Meru AP's that were donated to our club. This project exists to serve as a repository of any information we obtain during our quest to shoehorn OpenWrt on the hardware.

Notes:
* Units use standard 3.5mm 3-pole Headphone Jack for serial port. It is 5 Volt tolerant and does not require a level converter.
* Units run a custom version of RHEL and appear to use uBoot for the bootloader.


Wiring of Serial Cable
----

|____________________
| GND    | TX  | RX  \
|________|_____|_____/
|

Hardware Specs: Models AP332i/AP332e (internal antenna/external antenna)
------
* CPU
  * MCP8378E VRANGA
      * PowerPC based
      * 800/400 MHZ
      * QQTA1248

* External I/O
    * Gigabit Ethernet
    * Gigabit Ethernet w/POE In
    * 3.5mm Serial
    * 12V Power

* Internal I/O
    * Mini PCIE (X2) | 2.4 Ghz and 5 Ghz radios (3x3)





Written by mixadj
