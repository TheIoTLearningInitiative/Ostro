# Ostro
Ostro Project

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
xe1gyq@jessie:~/Downloads/ostro/toFlash$ ./flashall.sh 

```