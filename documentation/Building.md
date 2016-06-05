# Building

> The ostro-os repository is a combination of several different components in a single repository. It contains everything that is needed to build Ostro OS. [Github Ostro OS](https://github.com/ostroproject/ostro-os)

## Base Images

> ostro-image
> > The default image. Contains all programming runtimes

> ostro-image-dev
> > The same as ostro-image, plus build and debugging tools

> ostro-image-minimal
> > A smaller image which still has the core OS, but none of the optional runtimes

## Intel Edison

```sh
xe1gyq@jessie:~$ mkdir ostro
xe1gyq@jessie:~$ cd ostro/
```

```sh
xe1gyq@jessie:~/ostro$ git clone https://github.com/ostroproject/ostro-os.git
Cloning into 'ostro-os'...
remote: Counting objects: 391671, done.
remote: Compressing objects: 100% (3054/3054), done.
remote: Total 391671 (delta 2035), reused 329 (delta 329), pack-reused 388238
Receiving objects: 100% (391671/391671), 144.42 MiB | 205.00 KiB/s, done.
Resolving deltas: 100% (253541/253541), done.
Checking connectivity... done.
Checking out files: 100% (9520/9520), done.
```

```sh
xe1gyq@jessie:~/ostro$ cd ostro-os/
xe1gyq@jessie:~/ostro/ostro-os$ source oe-init-build-env
You had no conf/local.conf file. This configuration file has therefore been
created for you with some default values. You may wish to edit it to, for
example, select a different MACHINE (target hardware). See conf/local.conf
for more information as common configuration options are commented.

You had no conf/bblayers.conf file. This configuration file has therefore been
created for you with some default values. To add additional metadata layers
into your configuration please add entries to conf/bblayers.conf.

The Yocto Project has extensive documentation about OE including a reference
manual which can be found at:
    http://yoctoproject.org/documentation

For more information about OpenEmbedded see their website:
    http://www.openembedded.org/


### Shell environment set up for builds. ###

You can now run 'bitbake <target>'

Common targets are:
    ostro-image
    ostro-image-dev
    core-image-minimal
    meta-toolchain
    adt-installer
    meta-ide-support

Common targets are:
    ostro-image-noswupd (when building without swupd,
                         the recommended mode for local image building)
    ostro-image-swupd   (when building with swupd, the recommended mode
                         for deployment)

We recommend to use VirtualBox if you wish to run an Ostro image in a
virtual environment. Please check the doc/howtos/booting-and-installation.rst
technical note for more information.
```

```sh
xe1gyq@jessie:~/ostro/ostro-os/build$ ls
conf
xe1gyq@jessie:~/ostro/ostro-os/build$ nano conf/local.conf
```

```sh
...
#
# Machine Selection
#
# You need to select a specific machine to target the build with. There are a selection
# of several hardware platforms that are supported:
#
# For MinnowBoard and Gigabyte GB-BXBT-3825:
#MACHINE ?= "intel-corei7-64"
#
# For Intel Galileo Gen 2:
#MACHINE ?= "intel-quark"
# 
# For Intel Edison:
MACHINE ?= "edison"
# 
# For BeagleBone Black:
#MACHINE ?= "beaglebone"
# 
# This sets the default machine to be "intel-corei7-64" if no other machine is selected:
#MACHINE ??= "intel-corei7-64"
...
#PACKAGECONFIG_append_pn-qemu-native = " sdl"
#PACKAGECONFIG_append_pn-nativesdk-qemu = " sdl"
#ASSUME_PROVIDED += "libsdl-native"
...
```

```sh
....
# An explicit choice must be made between building Ostro OS
# development images and production images. See
# doc/howtows/building-images.rst for further instructions.

# Ostro OS development images get built when uncommenting the
# following line. Do not do this in production! The resulting images
# are not secure.
#
require conf/distro/include/ostro-os-development.inc

# When building production images, configure IMA signing
# as described in meta-integrity/README.md if IMA is enabled
# and uncomment the following line.
#
#require conf/distro/include/ostro-os-production.inc
...
```

```sh
xe1gyq@jessie:~/ostro/ostro-os/build$ # old bitbake ostro-image-dev
xe1gyq@jessie:~/ostro/ostro-os/build$ bitbake -k ostro-image-noswupd
xe1gyq@jessie:~/ostro-os/build$ bitbake -k ostro-image-noswupd
NOTE: /home/xe1gyq/ostro-os/meta-java/recipes-core/openjdk/openjre-8_72b05.bb: base_contains is deprecated, please use bb.utils.contains instead.
NOTE: /home/xe1gyq/ostro-os/meta-java/recipes-core/openjdk/openjdk-8_72b05.bb: base_contains is deprecated, please use bb.utils.contains instead.
NOTE: /home/xe1gyq/ostro-os/meta-java/recipes-core/openjdk/openjdk-8-native_72b05.bb: base_contains is deprecated, please use bb.utils.contains instead.
NOTE: /home/xe1gyq/ostro-os/meta-java/recipes-core/icedtea/icedtea7-native_2.1.3.bb: base_contains is deprecated, please use bb.utils.contains instead.
NOTE: /home/xe1gyq/ostro-os/meta-java/recipes-core/icedtea/icedtea7-native_2.1.3.bb: base_contains is deprecated, please use bb.utils.contains instead.
...
Parsing recipes:  19% |############                                                    | ETA:  00:06:32
...
Build Configuration:
BB_VERSION        = "1.31.0"
BUILD_SYS         = "i686-linux"
NATIVELSBSTRING   = "Debian-8.3"
TARGET_SYS        = "i686-ostro-linux"
MACHINE           = "edison"
DISTRO            = "ostro"
DISTRO_VERSION    = "1.0+snapshot-20160605"
TUNE_FEATURES     = "m32 edison"
TARGET_FPU        = ""
meta-ostro-fixes  
meta              
meta-selftest     
meta-intel        
meta-ostro        
meta-oic          
meta-security-smack 
meta-security-framework 
meta-integrity    
meta-intel-iot-middleware 
meta-ostro-bsp    
meta-edison-bsp   
meta-iot-web      
meta-yocto-bsp    
meta-iotqa        
meta-appfw        
meta-security-isafw 
meta-swupd        
meta-gnome        
meta-networking   
meta-oe           
meta-python       
meta-java         
meta-soletta      = "master:13d93e44844452112bf3653537e10007eecf4865"
...
NOTE: Fetching uninative binary shim from http://downloads.yoctoproject.org/releases/uninative/1.1/i686-nativesdk-libc.tar.bz2;sha256sum=1973aa8d07ba4fdae197ea3ffba1274c57ff7923679c364ec8e2b66c73483234
NOTE: Preparing RunQueue
NOTE: Checking sstate mirror object availability (for 1020 objects)
NOTE: Executing SetScene Tasks
Currently 2 running tasks (68 of 1030):
0: linux-firmware-1_144.0+gitAUTOINC+80d463be82-r0 do_populate_sysroot_setscene (pid 21300)
1: linux-firmware-1_144.0+gitAUTOINC+80d463be82-r0 do_package_write_ipk_setscene (pid 22299)
...
Currently 2 running tasks (706 of 1030):
0: glibc-locale-2.24-r0 do_package_write_ipk_setscene (pid 3247)
1: u-boot-fw-utils-edison-2014.04-1-r0 do_packagedata_setscene (pid 27968)
...
NOTE: Executing RunQueue Tasks
Currently 1 running tasks (2722 of 2805):
0: linux-yocto-edison-3.10.98+gitAUTOINC+2e4ace5b68-r0 do_kernel_checkout (pid 21120)
...
```

After 12 hours ...

```sh
meta-soletta      = "master:13d93e44844452112bf3653537e10007eecf4865"

NOTE: Fetching uninative binary shim from http://downloads.yoctoproject.org/releases/uninative/1.1/i686-nativesdk-libc.tar.bz2;sha256sum=1973aa8d07ba4fdae197ea3ffba1274c57ff7923679c364ec8e2b66c73483234
NOTE: Preparing RunQueue
NOTE: Checking sstate mirror object availability (for 1020 objects)
NOTE: Executing SetScene Tasks
NOTE: Executing RunQueue Tasks
WARNING: ostro-image-noswupd-1.0-r0 do_rootfs: The license listed Intel-OBL-Binary-Firmware-License was not in the licenses collected for recipe mcu-fw-bin
WARNING: ostro-image-noswupd-1.0-r0 do_rootfs: The license listed Intel-OBL-Binary-Firmware-License was not in the licenses collected for recipe mcu-fw-load
WARNING: ostro-image-noswupd-1.0-r0 do_rootfs: [log_check] ostro-image-noswupd: found 2 warning messages in the logfile:
[log_check] WARNING: The license listed Intel-OBL-Binary-Firmware-License was not in the licenses collected for recipe mcu-fw-bin
[log_check] WARNING: The license listed Intel-OBL-Binary-Firmware-License was not in the licenses collected for recipe mcu-fw-load

NOTE: Tasks Summary: Attempted 2805 tasks of which 1782 didn't need to be rerun and all succeeded.

Summary: There were 3 WARNING messages shown.
xe1gyq@jessie:~/ostro-os/build$  
```

## Issues

### local.conf editing, building production and development images

```sh
xe1gyq@jessie:~/ostro/ostro-os/build$ bitbake ostro-image-dev
ERROR: local.conf must be explicitly edited to select between building
production and development images. See the comments in local.conf.sample
and doc/howtos/building-images.rst.

Summary: There was 1 ERROR message shown, returning a non-zero exit code.
```

Fixed by commenting line below under __conf/local.conf__

```sh
xe1gyq@jessie:~/ostro/ostro-os/build$ nano conf/local.conf
#DISTRO ?= "ostro"
```

### libsdl-native

```sh
xe1gyq@jessie:~/ostro/ostro-os/build$ bitbake ostro-image-dev
NOTE: Your conf/bblayers.conf has been automatically updated.
ERROR:  OE-core's config sanity checker detected a potential misconfiguration.
    Either fix the cause of this error or at your own risk disable the checker (see sanity.conf).
    Following is the list of potential problems / advisories:

    libsdl-native is set to be ASSUME_PROVIDED but sdl-config can't be found in PATH. Please either install it, or configure qemu not to require sdl.

Summary: There was 1 ERROR message shown, returning a non-zero exit code.
```

Fixed by commenting lines below under __conf/local.conf__

```sh
xe1gyq@jessie:~/ostro/ostro-os/build$ nano conf/local.conf
#PACKAGECONFIG_append_pn-qemu-native = " sdl"
#PACKAGECONFIG_append_pn-nativesdk-qemu = " sdl"
#ASSUME_PROVIDED += "libsdl-native"
```

### clr-systemd-config

```sh
xe1gyq@jessie:~/ostro/ostro-os/build$ bitbake ostro-image
xe1gyq@jessie:~/ostro/ostro-os/build$ bitbake ostro-image-dev
Loading cache: 100% |#####################################################################################| ETA:  00:00:00
Loaded 2579 entries from dependency cache.
NOTE: Resolving any missing task queue dependencies
ERROR: Nothing RPROVIDES 'clr-systemd-config' (but /home/xe1gyq/ostro/ostro-os/meta-ostro/recipes-swupd/packagegroups/packagegroup-swupd.bb RDEPENDS on or otherwise requires it)
ERROR: clr-systemd-config was skipped: missing required distro feature 'systemd' (not in DISTRO_FEATURES)
NOTE: Runtime target 'clr-systemd-config' is unbuildable, removing...
Missing or unbuildable dependency chain was: ['clr-systemd-config']
NOTE: Runtime target 'packagegroup-swupd' is unbuildable, removing...
Missing or unbuildable dependency chain was: ['packagegroup-swupd', 'clr-systemd-config']
ERROR: Required build target 'ostro-image-dev' has no buildable providers.
Missing or unbuildable dependency chain was: ['ostro-image-dev', 'packagegroup-swupd', 'clr-systemd-config']

Summary: There were 2 ERROR messages shown, returning a non-zero exit code.
```

```sh
|  Adding system startup for /home/xe1gyq/ostro/ostro-os/build/tmp-glibc/work/edison-oe-linux/sysvinit/2.88dsf-r14/image/etc/init.d/bootlogd.
|  Adding system startup for /home/xe1gyq/ostro/ostro-os/build/tmp-glibc/work/edison-oe-linux/sysvinit/2.88dsf-r14/image/etc/init.d/stop-bootlogd.
| chown: invalid user: 'root.shutdown'
| WARNING: exit code 1 from a shell command.
| ERROR: Function failed: do_install (log file is located at /home/xe1gyq/ostro/ostro-os/build/tmp-glibc/work/edison-oe-linux/sysvinit/2.88dsf-r14/temp/log.do_install.13864)
ERROR: Task 696 (/home/xe1gyq/ostro/ostro-os/meta/recipes-core/sysvinit/sysvinit_2.88dsf.bb, do_install) failed with exit code '1'
NOTE: Tasks Summary: Attempted 1210 tasks of which 1205 didn't need to be rerun and 1 failed.
Waiting for 0 running tasks to finish:

Summary: 1 task failed:
  /home/xe1gyq/ostro/ostro-os/meta/recipes-core/sysvinit/sysvinit_2.88dsf.bb, do_install
Summary: There was 1 ERROR message shown, returning a non-zero exit code.
```
