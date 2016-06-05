# Package Management

```sh
xe1gyq@jessie:~/ostro-os/build$ nano conf/local.conf
```

```sh
# Package Management configuration
# 
# This variable lists which packaging formats to enable. Multiple package backends
# can be enabled at once and the first item listed in the variable will be used
# to generate the root filesystems.
# Options are:
#  - 'package_deb' for debian style deb files
#  - 'package_ipk' for ipk files are used by opkg (a debian style embedded package manager)
#  - 'package_rpm' for rpm style packages
# E.g.: PACKAGE_CLASSES ?= "package_rpm package_deb package_ipk"
# We default to ipk because it is faster/smaller and good enough for
# image creation. On-device package management is disabled by default
# and thus the additional features offered for that by rpm/deb do not
# matter.
PACKAGE_CLASSES ?= "package_ipk"
```

```sh
xe1gyq@jessie:~/ostro-os/build$ bitbake -k ostro-image-swupd
NOTE: /home/xe1gyq/ostro-os/meta-java/recipes-core/openjdk/openjre-8_72b05.bb: base_contains is deprecated, please use bb.utils.contains instead.
NOTE: /home/xe1gyq/ostro-os/meta-java/recipes-core/openjdk/openjdk-8-native_72b05.bb: base_contains is deprecated, please use bb.utils.contains instead.
NOTE: /home/xe1gyq/ostro-os/meta-java/recipes-core/openjdk/openjdk-8_72b05.bb: base_contains is deprecated, please use bb.utils.contains instead.
NOTE: /home/xe1gyq/ostro-os/meta-java/recipes-core/icedtea/icedtea7-native_2.1.3.bb: base_contains is deprecated, please use bb.utils.contains instead.
NOTE: /home/xe1gyq/ostro-os/meta-java/recipes-core/icedtea/icedtea7-native_2.1.3.bb: base_contains is deprecated, please use bb.utils.contains instead.
NOTE: /home/xe1gyq/ostro-os/meta-java/recipes-core/icedtea/icedtea7-native_2.1.3.bb: base_contains is deprecated, please use bb.utils.contains instead.
NOTE: /home/xe1gyq/ostro-os/meta-java/recipes-core/icedtea/icedtea7-native_2.1.3.bb: base_contains is deprecated, please use bb.utils.contains instead.
NOTE: /home/xe1gyq/ostro-os/meta-ostro-bsp/meta-edison-bsp/recipes-connectivity/bluetooth-rfkill-event/bluetooth-rfkill-event_1.0.bb: base_contains is deprecated, please use bb.utils.contains instead.
NOTE: /home/xe1gyq/ostro-os/meta-soletta/recipes-modules/libmicrohttpd/libmicrohttpd_0.9.49.bb: base_contains is deprecated, please use bb.utils.contains instead.
NOTE: /home/xe1gyq/ostro-os/meta-soletta/recipes-modules/libmicrohttpd/libmicrohttpd_0.9.49.bb: base_contains is deprecated, please use bb.utils.contains instead.
Parsing recipes: 100% |################################################################| Time: 00:02:14
Parsing of 2112 .bb files complete (0 cached, 2112 parsed). 2747 targets, 380 skipped, 1 masked, 0 errors.
NOTE: Resolving any missing task queue dependencies
NOTE: multiple providers are available for runtime java2-runtime (openjre-8, openjdk-8)
NOTE: consider defining a PREFERRED_RPROVIDER entry to match java2-runtime

Build Configuration:
BB_VERSION        = "1.31.0"
BUILD_SYS         = "i686-linux"
NATIVELSBSTRING   = "universal"
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

NOTE: Preparing RunQueue
NOTE: Checking sstate mirror object availability (for 637 objects)
NOTE: Executing SetScene Tasks
NOTE: Executing RunQueue Tasks
Currently 2 running tasks (594 of 4280):
0: fastjar-native-0.98-r1 do_configure (pid 29665)
1: jikes-native-1.22-r0 do_compile (pid 32517)

```