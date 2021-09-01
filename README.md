[![Build Status](https://travis-ci.com/hanwckf/rt-n56u.svg?branch=master)](https://travis-ci.com/hanwckf/rt-n56u)
![GitHub All Releases](https://img.shields.io/github/downloads/hanwckf/rt-n56u/total)
[![release](https://img.shields.io/github/release/hanwckf/rt-n56u.svg)](https://github.com/hanwckf/rt-n56u/releases)

# README #

### Demo ###
[![2oPwfzW.png](https://i.imgur.com/2oPwfzW.png)](https://i.imgur.com/2oPwfzW.png)


### Big Thanks ###
* https://github.com/yuos-bit/Padavan

***

- Login:
```shell 
10.32.0.1 
user: admin
password: admin
```

***

### Build Firmware ###

* https://github.com/irisvn/xiaomi-padavan-docker

### How to install padavan from stock? ###

1- Use https://github.com/acecilia/OpenWRTInvasion to gain telnet access.

2- Make Backup fullflash 
Use file: https://github.com/irisvn/Padavan/releases/download/v3.4.3.9/mi4c_factory_backup_and_flash.zip

Run file "Backup.bat"
Data will save to "Data" Folder: backup.bin and eeprom.bin (save them)

3- Use any ftp client to upload breed-mt7688-reset38.bin to /tmp

https://github.com/irisvn/Padavan/releases/download/v3.4.3.9/breed-mt7688-reset38.bin

4- Run ``` mtd -r write /tmp/breed-mt7688-reset38.bin Bootloader ``` on shell to install bootloader.

5- Login breed web 192.168.1.1 with reset clamped when the router is turned on. 

6- Upload from breed web padavan:
++ eeprom.bin (from step 2)
++ MI-4C_3.4.3.9-099-English.trx 

7- Go to 10.32.0.1  on your browser
