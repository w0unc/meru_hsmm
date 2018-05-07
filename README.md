
# meru_hsmm
We have a bunch of Meru AP's that were donated to our club. This project exists to serve as a repository of any information we obtain during our quest to shoehorn OpenWrt on the hardware.

Notes:
* Units use standard 3.5mm 3-pole Headphone Jack for serial port. It is 5 Volt tolerant and does not require a level converter.
* Units run a custom version of RHEL and appear to use uBoot for the bootloader.



Hardware Specs: Models AP332i/AP332e (internal antenna/external antenna)
------
* CPU
  * MCP8378E VRANGA
      * PowerPC based
      * 800/400 MHZ
      * QQTA1248
* Memory
  * DRAM 256 MB
  * [H5PS5182GFR](https://www.skhynix.com/product/filedata/fileDownload.do?seq=1906) (x4)
    * Modules are 512Mb

* Flash
  * 32 MB
  * [S29GL256P90TFCR20](http://www.cypress.com/part/s29gl256p90tfcr20)
* PCIE
  * Broadcom BCM 4331 (2.4 Ghz)
  * Broadcom BCM 4331 (5 Ghz)

* Ethernet Controllers
  * [SimpliPhy vsc8601](https://media.digikey.com/pdf/Data%20Sheets/Vitesse%20PDFs/VSC8601,8641%20Prod%20Brief.pdf) (x2)

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

Notes
-----

### Getting root

Once the os is booted, you can run a limited number of commands in the shell that are incompletely sanitized. e.g.:

`system exec cat /etc/exports | killall Atsmain` to drop to a shell.

Something causes the OS to reboot within a few seconds once it realizes Atsmain is no longer running.

There's also apparently an undocumented `shell` command that can present you with a login screen if you have credentials. The only account with a password is:

`root:$1$oxduCrHo$3LQZUCnlYFmBtfsWFEJB11:11851:0:99999:7:::`
`The password is meru2002`
