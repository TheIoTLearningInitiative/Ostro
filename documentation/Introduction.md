Introduction
==
> Welcome to the Ostro™ Project! It is an open source developed, Linux*-based operating system tailored for IoT smart devices and built with security in mind. With Ostro OS you won't need to force-fit a general Linux OS to suit your IoT device or write your own OS.

> The Ostro™ OS is a scalable open source operating system tailored specifically for IoT smart devices. Out of the box, we provide an OS developer image ready to install on a USB stick or SD card, boot, and then use to learn about the Ostro OS. With this developer image you can build and test applications written for the Ostro OS, and then later build a clean production image for deploying on your devices.

- [Ostro Project Homepage](https://ostroproject.org/)

Supported Platforms

- Beaglebone
- Intel Edison
- Intel Core i7-64
- Intel Quark

## Ostro Documentation

> These technical documents and architecture guides help you learn more about the Ostro OS and how to use it to create and deploy IoT applications.

- [Ostro All Documentation](https://ostroproject.org/documentation/)
- [Ostro Articles](https://ostroproject.org/documentation/howtos/howtos.html)
- [Ostro Getting Started](https://ostroproject.org/documentation/quick_start/quick_start.html)

## Downloading a Pre-Built Ostro OS Image

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

## Booting and Installing an Ostro™ OS Image, Intel Edison, Host Side

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
[    1.670504] Kernel panic - not syncing: VFS: Unable to mount root fs on unknown-block(179,8)
[    1.670669] emmc_ipanic: panic notified
[    1.670705] emmc_ipanic: Crash partition in use!
[    1.670775] ------------[ cut here ]------------
[    1.670833] WARNING: at /var/lib/jenkins/ostro-worker-15-slot-1-IvKXr/ostro-os/build/tmp-glibc/work-shared/edison/kern)
[    1.670929] Modules linked in:
[    1.670971] CPU: 0 PID: 1 Comm: swapper/0 Not tainted 3.10.98-yocto-standard #1
[    1.671021] Hardware name: Intel Corporation Merrifield/BODEGA BAY, BIOS 466 2014.06.23:19.20.05
[    1.671077]  00000000 00000000 f6889d64 c18b9a03 f6889d8c c123fc5e c1ab08ad c1aa1bfc
[    1.671174]  0000007b c121f6e7 c121f6e7 f70024c0 00000001 f6ff54c0 f6889d9c c123fd22
[    1.671268]  00000009 00000000 f6889da4 c121f6e7 f6889dc0 c127c1d4 ffff8b71 00000000
[    1.671363] Call Trace:
[    1.671409]  [<c18b9a03>] dump_stack+0x16/0x18
[    1.671459]  [<c123fc5e>] warn_slowpath_common+0x5e/0x80
[    1.671509]  [<c121f6e7>] ? native_smp_send_reschedule+0x57/0x60
[    1.671561]  [<c121f6e7>] ? native_smp_send_reschedule+0x57/0x60
[    1.671616]  [<c123fd22>] warn_slowpath_null+0x22/0x30
[    1.671665]  [<c121f6e7>] native_smp_send_reschedule+0x57/0x60
[    1.671720]  [<c127c1d4>] trigger_load_balance+0x144/0x1f0
[    1.671774]  [<c1270c4d>] scheduler_tick+0xdd/0x110
[    1.671823]  [<c1250846>] update_process_times+0x56/0x70
[    1.671873]  [<c1294496>] tick_sched_handle.isra.11+0x26/0x60
[    1.671924]  [<c129450a>] tick_sched_timer+0x3a/0x70
[    1.671974]  [<c1265748>] ? __remove_hrtimer+0x38/0x90
[    1.672024]  [<c1265bab>] __run_hrtimer+0x7b/0x230
[    1.672070]  [<c12944d0>] ? tick_sched_handle.isra.11+0x60/0x60
[    1.672126]  [<c1266a68>] hrtimer_interrupt+0x208/0x2a0
[    1.672175]  [<c18b8f48>] ? printk+0x1c/0x1e
[    1.672227]  [<c18c3918>] smp_apic_timer_interrupt+0x58/0x8d
[    1.672279]  [<c14c3e44>] ? trace_hardirqs_off_thunk+0xc/0x18
[    1.672331]  [<c18be3f5>] apic_timer_interrupt+0x39/0x40
[    1.672384]  [<c124007b>] ? perf_trace_console+0xcb/0x110
[    1.672436]  [<c14c00d8>] ? format_decode+0x358/0x3d0
[    1.672484]  [<c18b8ecf>] ? panic+0x129/0x164
[    1.672533]  [<c1c25dfb>] mount_block_root+0x1fc/0x204
[    1.672585]  [<c132b6fd>] ? SyS_mknod+0x2d/0x30
[    1.672631]  [<c1c25f29>] mount_root+0x4f/0x57
[    1.672678]  [<c1c26071>] prepare_namespace+0x140/0x171
[    1.672727]  [<c1c25b35>] kernel_init_freeable+0x18b/0x198
[    1.672780]  [<c18ac8c0>] kernel_init+0x10/0x160
[    1.672828]  [<c18c3237>] ret_from_kernel_thread+0x1b/0x28
[    1.672878]  [<c18ac8b0>] ? rest_init+0x80/0x80
[    1.672918] ---[ end trace f79745a19c22847d ]---
```

## Booting and Installing an Ostro™ OS Image, Intel Edison, Device Side

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

