# Smartest
======================================================
Smartest v6.3  (August, 2015)

 **This program is deprecated and not actively developed anymore.**
 
 You can find the new repository full supported on [device-inventory](https://github.com/eReuse/device-inventory).
______________________
Documentation
======================
 
 This README is for the configuration and use of Smartest

______________________
Release Notes
======================

 Only support SATA hard disks. [Issue #1](https://github.com/eReuse/Smartest/issues/1)
 
_____________________
Installation
======================

 Install the next files from the repository to "/usr/share/smartest/*".

````
       - smartest
                |- bin
                |    |- smartest
                |- etc
                     |- menu_ca.properties
                     |- menu_en.properties
                     |- menu_es.properties
````

 Smartest needs `smartmontools` package:
 
 * Installation of `smartmontools` on Ubuntu.
````
sudo apt-get install smartmontools
````

______________________
Usage
======================

 To run this application, you need to install [DeviceInventory](https://github.com/eReuse/DeviceInventory)  to run `smartest`.

 This program reads the configuration on **config.ini**:
 
 * Y = Asks what test want to do.
 * 1 = To do a quick HDD check without asking to user.
 * 2 = To do a long HDD check without asking to user.
 * N = Do not ask or check.

 (If you choise any test, *DeviceInventory* will wait until the test finish.)

 When the check is finished, it will be saved to `/usr/share/donator/etc/data.ini`
 where `donator` import the results of the test.
 
______________________
Support
======================

 For any support or report, please contact to: adrias@ereuse.org
