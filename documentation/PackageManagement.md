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