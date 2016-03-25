# Architecture

```sh
OSTRO_LAYERS = " \
  /home/xe1gyq/ostro/ostro-os/meta-ostro-fixes \
  /home/xe1gyq/ostro/ostro-os/meta \
  /home/xe1gyq/ostro/ostro-os/meta-selftest \
  /home/xe1gyq/ostro/ostro-os/meta-intel \
  /home/xe1gyq/ostro/ostro-os/meta-ostro \
  /home/xe1gyq/ostro/ostro-os/meta-oic \
  /home/xe1gyq/ostro/ostro-os/meta-intel-iot-security/meta-security-smack \
  /home/xe1gyq/ostro/ostro-os/meta-intel-iot-security/meta-security-framework \
  /home/xe1gyq/ostro/ostro-os/meta-intel-iot-security/meta-integrity \
  /home/xe1gyq/ostro/ostro-os/meta-intel-iot-middleware \
  /home/xe1gyq/ostro/ostro-os/meta-ostro-bsp \
  /home/xe1gyq/ostro/ostro-os/meta-ostro-bsp/meta-edison-bsp \
  /home/xe1gyq/ostro/ostro-os/meta-iot-web \
  /home/xe1gyq/ostro/ostro-os/meta-yocto/meta-yocto-bsp \
  /home/xe1gyq/ostro/ostro-os/meta-iotqa \
  /home/xe1gyq/ostro/ostro-os/meta-appfw \
  /home/xe1gyq/ostro/ostro-os/meta-security-isafw \
  "

# OSTRO_LAYERS += "/home/xe1gyq/ostro/ostro-os/meta-openembedded/meta-efl"
# OSTRO_LAYERS += "/home/xe1gyq/ostro/ostro-os/meta-openembedded/meta-filesystems"
# OSTRO_LAYERS += "/home/xe1gyq/ostro/ostro-os/meta-openembedded/meta-gnome"
# OSTRO_LAYERS += "/home/xe1gyq/ostro/ostro-os/meta-openembedded/meta-gpe"
# OSTRO_LAYERS += "/home/xe1gyq/ostro/ostro-os/meta-openembedded/meta-initramfs"
# OSTRO_LAYERS += "/home/xe1gyq/ostro/ostro-os/meta-openembedded/meta-multimedia"
OSTRO_LAYERS += "/home/xe1gyq/ostro/ostro-os/meta-openembedded/meta-networking"
OSTRO_LAYERS += "/home/xe1gyq/ostro/ostro-os/meta-openembedded/meta-oe"
# OSTRO_LAYERS += "/home/xe1gyq/ostro/ostro-os/meta-openembedded/meta-perl"
OSTRO_LAYERS += "/home/xe1gyq/ostro/ostro-os/meta-openembedded/meta-python"
# OSTRO_LAYERS += "/home/xe1gyq/ostro/ostro-os/meta-openembedded/meta-ruby"
# OSTRO_LAYERS += "/home/xe1gyq/ostro/ostro-os/meta-openembedded/meta-systemd"
# OSTRO_LAYERS += "/home/xe1gyq/ostro/ostro-os/meta-openembedded/meta-webserver"
# OSTRO_LAYERS += "/home/xe1gyq/ostro/ostro-os/meta-openembedded/meta-xfce"
# OSTRO_LAYERS += "/home/xe1gyq/ostro/ostro-os/meta-openembedded/toolchain-layer"
OSTRO_LAYERS += "/home/xe1gyq/ostro/ostro-os/meta-java"
OSTRO_LAYERS += "/home/xe1gyq/ostro/ostro-os/meta-soletta"

```

{% include "documentation/Running.md" %}

