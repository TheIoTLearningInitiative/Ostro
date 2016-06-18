Sandbox
==

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


{% include "Running.md" %}