# SwUpd

- ostro-image-noswupd (when building without swupd, the recommended mode for local image building)
- ostro-image-swupd   (when building with swupd, the recommended mode for deployment)

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