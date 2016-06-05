# Flashing

# Intel Edison, Flashing an Ostro™ OS Image, Host Side

```sh
xe1gyq@jessie:~/Downloads/ostro/toFlash$ ./flashall.sh 
Image name: ostro-image-noswupd
Using U-Boot target: edison-blankcdc
Now waiting for dfu device 8087:0a99
Please plug and reboot the board
Flashing IFWI
Download	[=========================] 100%      4194304 bytes
Download	[=========================] 100%      4194304 bytes
Flashing U-Boot
Download	[=========================] 100%       237568 bytes
Flashing U-Boot Environment
Download	[=========================] 100%        65536 bytes
Flashing U-Boot Environment Backup
Download	[=========================] 100%        65536 bytes
Rebooting to apply partition changes
Now waiting for dfu device 8087:0a99
Flashing boot partition (kernel)
Download	[=========================] 100%     33554432 bytes
Flashing update partition
Download	[=========================] 100%    805306368 bytes
Flashing rootfs, (it can take up to 5 minutes... Please be patient)

```