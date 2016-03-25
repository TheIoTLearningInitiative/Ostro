Building
==

- [Github Ostro OS ](https://github.com/ostroproject/ostro-os)

```sh
xe1gyq@jessie:~$ mkdir ostro
xe1gyq@jessie:~$ cd ostro/
xe1gyq@jessie:~/ostro$ git clone https://github.com/ostroproject/ostro-os.git
Cloning into 'ostro-os'...
remote: Counting objects: 373987, done.
remote: Compressing objects: 100% (624/624), done.
remote: Total 373987 (delta 401), reused 129 (delta 129), pack-reused 373219
Receiving objects: 100% (373987/373987), 135.33 MiB | 185.00 KiB/s, done.
Resolving deltas: 100% (241720/241720), done.
Checking connectivity... done.
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

We recommend to use VirtualBox if you wish to run an Ostro image in a
virtual environment. Please check the doc/howtos/booting-and-installation.rst
technical note for more information.
xe1gyq@jessie:~/ostro/ostro-os/build$ ls
bitbake.lock  cache  conf  tmp-glibc
xe1gyq@jessie:~/ostro/ostro-os/build$ nano conf/local.conf
# For Intel Edison:
MACHINE ?= "edison"
...
#DISTRO ?= "ostro"
...
#PACKAGECONFIG_append_pn-qemu-native = " sdl"
#PACKAGECONFIG_append_pn-nativesdk-qemu = " sdl"
#ASSUME_PROVIDED += "libsdl-native"
...
xe1gyq@jessie:~/ostro/ostro-os/build$ bitbake ostro-image-dev

```

### Base Images

> ostro-image
> > The default image. Contains all programming runtimes

> ostro-image-dev
> > The same as ostro-image, plus build and debugging tools

> ostro-image-minimal
> > A smaller image which still has the core OS, but none of the optional runtimes