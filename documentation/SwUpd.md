# SwUpd

> The [SoftWare UPDater](https://clearlinux.org/features/software-update) — swupd — from [Clear Linux](https://clearlinux.org/) provides a new way of adding functionality to and updating a Linux-based OS. [Meta layer for swupd software-update](http://git.yoctoproject.org/cgit/cgit.cgi/meta-swupd/tree/docs/Guide.md)

- [About software update](https://clearlinux.org/documentation/swupdate_about_sw_update.html)
- [How to run the updater](https://clearlinux.org/documentation/swupdate_how_to_run_the_updater.html)

- ostro-image-noswupd (when building without swupd, the recommended mode for local image building)
- ostro-image-swupd   (when building with swupd, the recommended mode for deployment)

# Bundles

- [Bundles overview](https://clearlinux.org/documentation/bundles_overview.html)

![Clear Linux Bundles Overview](https://clearlinux.org/documentation/_images/bundles_overview.png)

##

```sh
root@edison:~# ls /usr/share/clear/bundles
os-core    world-dev
root@edison:~# 
```

```sh
root@edison:~# swupd
Usage:
    swupd [OPTION...]
 or swupd [OPTION...] SUBCOMMAND [OPTION...]

Help Options:
   -h, --help              Show help options

Subcommands:
   bundle-add              Install a new bundle          
   bundle-remove           Uninstall a bundle            
   hashdump                Dumps the HMAC hash of a file 
   update                  Update to latest OS version   
   verify                  Verify content for OS version 
   check-update            Checks if a new OS version is available

To view subcommand options, run `swupd SUBCOMMAND --help'
root@edison:~# 
```

```sh
root@edison:~# swupd update
swupd-client software update 2.87
   Copyright (C) 2012-2015 Intel Corporation
   bsdiff portions Copyright Colin Percival, see COPYING file for details

Error: Network issue, unable to proceed with update
Update exiting.
root@edison:~# 
```

```sh
root@edison:~# swupd bundle-add editors
swupd-client bundle adder 2.87
   Copyright (C) 2012-2015 Intel Corporation
   bsdiff portions Copyright Colin Percival, see COPYING file for details

Cannot load official manifest MoM for version 4400
root@edison:~# 
```