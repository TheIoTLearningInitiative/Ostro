Introduction
==

## Download

```sh
xe1gyq@jessie:~/Downloads/ostro$ wget https://download.ostroproject.org/builds/ostro-os/2016-03-23_23-27-58-build-411/images/edison/ostro-image-dev-edison.toflash.tar.bz2
xe1gyq@jessie:~/Downloads$ wget https://download.ostroproject.org/builds/ostro-os/2016-03-23_23-27-58-build-411/images/edison/ostro-image-dev-edison.toflash.tar.bz2
--2016-03-24 22:36:55--  https://download.ostroproject.org/builds/ostro-os/2016-03-23_23-27-58-build-411/images/edison/ostro-image-dev-edison.toflash.tar.bz2
Resolving download.ostroproject.org (download.ostroproject.org)... 198.145.21.61, 2001:19d0:306:8::3
Connecting to download.ostroproject.org (download.ostroproject.org)|198.145.21.61|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 764412486 (729M) [application/x-bzip2]
Saving to: ‘ostro-image-dev-edison.toflash.tar.bz2’

ostro-image-dev-edi 100%[=====================>] 729.00M   753KB/s   in 15m 47ss

2016-03-24 22:52:43 (788 KB/s) - ‘ostro-image-dev-edison.toflash.tar.bz2’ saved [764412486/764412486]

xe1gyq@jessie:~/Downloads$ ls
xe1gyq@jessie:~/Downloads$ mv ostro-image-dev-edison.toflash.tar.bz2 ostro
xe1gyq@jessie:~/Downloads$ cd ostro/
xe1gyq@jessie:~/Downloads/ostro$ ls
ostro-image-dev-edison.toflash.tar.bz2
xe1gyq@jessie:~/Downloads/ostro$ tar xvf ostro-image-dev-edison.toflash.tar.bz2
toFlash/
toFlash/filter-dfu-out.js
toFlash/pft-config-edison.xml
toFlash/edison_ifwi-dbg-02-dfu.bin
toFlash/ostro-image-dev-edison.ext4
toFlash/edison_dnx_osr.bin
toFlash/edison_ifwi-dbg-05-dfu.bin
toFlash/edison_ifwi-dbg-03-dfu.bin
toFlash/edison_ifwi-dbg-06.bin
toFlash/edison_ifwi-dbg-02.bin
toFlash/edison_ifwi-dbg-01-dfu.bin
toFlash/edison_ifwi-dbg-03.bin
toFlash/u-boot-edison.bin
toFlash/ostro-image-dev-edison.update.hddimg
toFlash/ostro-image-dev-edison.hddimg
toFlash/u-boot-edison.img
toFlash/edison_ifwi-dbg-04-dfu.bin
toFlash/edison_ifwi-dbg-00-dfu.bin
toFlash/edison_ifwi-dbg-01.bin
toFlash/edison_dnx_fwr.bin
toFlash/u-boot-envs/
toFlash/u-boot-envs/edison-blankrndis.bin
toFlash/u-boot-envs/edison-ifwi.bin
toFlash/u-boot-envs/edison-blankcdc.bin
toFlash/u-boot-envs/edison-prod.bin
toFlash/helper/
toFlash/helper/images/
toFlash/helper/images/Edison-breakout-board.png
toFlash/helper/images/Edison-arduino-blink-led.png
toFlash/helper/images/Edison-arduino.png
toFlash/helper/helper.html
toFlash/edison_ifwi-dbg-06-dfu.bin
toFlash/edison_ifwi-dbg-05.bin
toFlash/edison_ifwi-dbg-00.bin
toFlash/edison_ifwi-dbg-04.bin
toFlash/package-list.txt
toFlash/FlashEdison.json
toFlash/flashall.bat
toFlash/flashall.sh
xe1gyq@jessie:~/Downloads/ostro$ cd toFlash/
```

## Flashing, Host Side

```sh
xe1gyq@jessie:~/Downloads/ostro/toFlash$ ./flashall.sh 

```

```sh
******************************
PSH KERNEL VERSION: b0182929
                WR: 20104000
******************************

SCU IPC: 0x800000d0  0xfffce92c

PSH miaHOB version: TNG.B0.VVBD.0000000c

microkernel built 10:14:01 Jan 13 2015

******* PSH loader *******
PCM page cache size = 192 KB 
Cache Constraint = 0 Pages
Arming IPC driver ..
Adding page store pool ..
PagestoreAddr(IMR Start Address) = 0x04899000
pageStoreSize(IMR Size)          = 0x00080000

*** Ready to receive application *** 


U-Boot 2014.04 (Mar 23 2016 - 10:35:12)

       Watchdog enabled
DRAM:  980.6 MiB
MMC:   tangier_sdhci: 0, tangier_sdhci: 1
In:    serial
Out:   serial
Err:   serial
Hit any key to stop autoboot:  0 
Target:blank
Partitioning already done...
Flashing already done...
GADGET DRIVER: usb_dnl_dfu
Card did not respond to voltage select!
** Bad device mmc 1 **
reading vmlinuz
5296624 bytes read in 131 ms (38.6 MiB/s)
Booting from emmc ...
Valid Boot Flag
Setup Size = 0x00003c00
Magic signature found
Using boot protocol version 2.0c
Linux kernel version 3.10.98-yocto-standard (jenkins@ostro-worker-15) #1 SMP PREEMPT Thu Mar 24 08:53:01 UTC 2016
Building boot_params at 0x00090000
Loading bzImage at address 00100000 (5281264 bytes)
Magic signature found
Kernel command line: "rootwait root=PARTUUID=012b3303-34ac-284d-99b4-34e03a2335f4 rootfstype=ext4 console=ttyMFD2 earlypr"

Starting kernel ...

[    0.612659] tpm_tis tpm_tis: tpm_transmit: tpm_send: error -5
[    0.612738] tpm_tis tpm_tis: A TPM error (-5) occurred attempting to determine the timeouts
[    0.612841] tpm_tis tpm_tis: tpm_transmit: tpm_send: error -5
[    0.612904] tpm_tis tpm_tis: Could not get TPM timeouts and durations
[    1.562079] pmic_ccsm pmic_ccsm: Error reading battery profile from battid frmwrk
[    1.571908] pmic_ccsm pmic_ccsm: Battery Over heat exception
[    1.571988] pmic_ccsm pmic_ccsm: Battery0 temperature inside boundary
```

## Flashing, Device Side

```sh

******************************
PSH KERNEL VERSION: b0182929
                WR: 20104000                                                 
******************************                                               
                                                                             
SCU IPC: 0x800000d0  0xfffce92c                                              
                                                                             
PSH miaHOB version: TNG.B0.VVBD.0000000c

microkernel built 10:14:01 Jan 13 2015

******* PSH loader *******
PCM page cache size = 192 KB 
Cache Constraint = 0 Pages
Arming IPC driver ..
Adding page store pool ..
PagestoreAddr(IMR Start Address) = 0x04899000
pageStoreSize(IMR Size)          = 0x00080000

*** Ready to receive application *** 


******************************
PSH KERNEL VERSION: b0182929
                WR: 20104000
******************************

SCU IPC: 0x800000d0  0xfffce92c

PSH miaHOB version: TNG.B0.VVBD.0000000c

microkernel built 10:14:01 Jan 13 2015

******* PSH loader *******
PCM page cache size = 192 KB 
Cache Constraint = 0 Pages
Arming IPC driver ..
Adding page store pool ..
PagestoreAddr(IMR Start Address) = 0x04899000
pageStoreSize(IMR Size)          = 0x00080000

*** Ready to receive application *** 


U-Boot 2014.04 (Mar 23 2016 - 10:35:12)

       Watchdog enabled
DRAM:  980.6 MiB
MMC:   tangier_sdhci: 0, tangier_sdhci: 1
In:    serial
Out:   serial
Err:   serial
Hit any key to stop autoboot:  0 
Target:blank
Partitioning already done...
Flashing already done...
GADGET DRIVER: usb_dnl_dfu
#
DFU complete CRC32: 0xd0a55b68
DOWNLOAD ... OK
Ctrl+C to exit ...
#
DFU complete CRC32: 0xd0a55b68
DOWNLOAD ... OK
Ctrl+C to exit ...
#
DFU complete CRC32: 0x15021025
DOWNLOAD ... OK
Ctrl+C to exit ...
#
DFU complete CRC32: 0x1a81e926
DOWNLOAD ... OK
Ctrl+C to exit ...
#
DFU complete CRC32: 0x1a81e926
DOWNLOAD ... OK
Ctrl+C to exit ...
resetting ...


******************************
PSH KERNEL VERSION: b0182929
                WR: 20104000
******************************

SCU IPC: 0x800000d0  0xfffce92c

PSH miaHOB version: TNG.B0.VVBD.0000000c

microkernel built 10:14:01 Jan 13 2015

******* PSH loader *******
PCM page cache size = 192 KB 
Cache Constraint = 0 Pages
Arming IPC driver ..
Adding page store pool ..
PagestoreAddr(IMR Start Address) = 0x04899000
pageStoreSize(IMR Size)          = 0x00080000

*** Ready to receive application *** 


U-Boot 2014.04 (Mar 23 2016 - 10:35:12)

       Watchdog enabled
DRAM:  980.6 MiB
MMC:   tangier_sdhci: 0, tangier_sdhci: 1
In:    serial
Out:   serial
Err:   serial
Writing to redundant MMC(0)... done
Writing to MMC(0)... done
Hit any key to stop autoboot:  0 
Target:blank
Partitioning using GPT
Writing GPT: success!
Saving Environment to MMC...
Writing to redundant MMC(0)... done
Flashing already done...
GADGET DRIVER: usb_dnl_dfu
####
DFU complete CRC32: 0x26075471
DOWNLOAD ... OK
Ctrl+C to exit ...
################################################################################################
DFU complete CRC32: 0x64a3179f
DOWNLOAD ... OK
Ctrl+C to exit ...
```

