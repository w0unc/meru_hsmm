# meru_hsmm
We have a bunch of Meru AP's that were donated to our club. This project exists to serve as a repository of any information we obtain during our quest to shoehorn OpenWrt on the hardware.

Notes:
* Units use standard 3.5mm 3-pole Headphone Jack for serial port. It is 5 Volt tolerant and does not require a level converter.
* Units run a custom version of RHEL and appear to use uBoot for the bootloader.

[W0UNC Slack Link](https://join.slack.com/w0unc/shared_invite/MTk2ODQxMzE3NTQzLTE0OTcyMTM3NDAtZjYzMzlkOWIzNQ) (Dies in 7 days)


Hardware Specs: Models AP332i/AP332e (internal antenna/external antenna)
------
* CPU
  * MCP8378E VRANGA
      * PowerPC based
      * 800/400 MHZ
      * QQTA1248
* Memory
  * DRAM 256 MB

* Flash
  * 32 MB

* PCIE
  * Broadcom BCM 4331 (2.4 Ghz)
  * Broadcom BCM 4331 (5 Ghz)

* External I/O
    * Gigabit Ethernet
    * Gigabit Ethernet w/POE In
    * 3.5mm Serial
    * 12V Power

* Internal I/O
    * Mini PCIE (X2) | 2.4 Ghz and 5 Ghz radios (3x3)


Software
-------
* Linux Kernel 2.6.25
  * PowerPC

Notes:
Hash of root password;

$1$oxduCrHo$3LQZUCnlYFmBtfsWFEJB11:11851:0:99999:7:::

limited command set in stock firmware
