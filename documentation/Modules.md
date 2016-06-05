# Modules

```sh
root@edison:~# lsmod
Module                  Size  Used by
xt_connmark            12659  2
iptable_nat            12867  0
nf_nat_ipv4            13039  1 iptable_nat
nf_nat                 24562  2 nf_nat_ipv4,iptable_nat
iptable_mangle         12615  1
spidev                 13370  0
usb_f_acm              14307  1
u_serial               18554  1 usb_f_acm
g_multi                66517  0
libcomposite           39152  2 usb_f_acm,g_multi
bcm_bt_lpm             13676  0
bcm4334x              586417  0
nf_conntrack_ipv6      13888  1
nf_defrag_ipv6         26022  1 nf_conntrack_ipv6
nf_conntrack_ipv4      19083  4
nf_defrag_ipv4         12601  1 nf_conntrack_ipv4
xt_tcpudp              12756  6
xt_conntrack           12664  2
iptable_filter         12706  1
ip6table_filter        12711  1
ip6_tables             17634  1 ip6table_filter
ip_tables              17806  3 iptable_filter,iptable_mangle,iptable_nat
x_tables               20879  8 ip6table_filter,ip_tables,xt_tcpudp,xt_conntrack,iptable_filter,xt_cons
root@edison:~# 
```

```sh
root@edison:~# find /lib/modules/* -name '*'
/lib/modules/3.10.98-yocto-standard
/lib/modules/3.10.98-yocto-standard/modules.symbols
/lib/modules/3.10.98-yocto-standard/modules.alias.bin
/lib/modules/3.10.98-yocto-standard/kernel
/lib/modules/3.10.98-yocto-standard/kernel/net
/lib/modules/3.10.98-yocto-standard/kernel/net/ipv4
/lib/modules/3.10.98-yocto-standard/kernel/net/ipv4/netfilter
/lib/modules/3.10.98-yocto-standard/kernel/net/ipv4/netfilter/ipt_CLUSTERIP.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/ipv4/netfilter/ip_tables.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/ipv4/netfilter/ipt_ah.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/ipv4/netfilter/iptable_security.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/ipv4/netfilter/iptable_mangle.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/ipv4/netfilter/nf_conntrack_ipv4.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/ipv4/netfilter/ipt_REJECT.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/ipv4/netfilter/iptable_nat.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/ipv4/netfilter/iptable_filter.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/ipv4/netfilter/iptable_raw.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/ipv4/netfilter/nf_defrag_ipv4.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/ipv4/netfilter/ipt_MASQUERADE.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/ipv4/netfilter/nf_nat_ipv4.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/ipv4/netfilter/ipt_ECN.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/nfc
/lib/modules/3.10.98-yocto-standard/kernel/net/nfc/hci
/lib/modules/3.10.98-yocto-standard/kernel/net/nfc/hci/hci.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/nfc/nfc.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/nfc/nci
/lib/modules/3.10.98-yocto-standard/kernel/net/nfc/nci/nci.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/ieee802154
/lib/modules/3.10.98-yocto-standard/kernel/net/ieee802154/ieee802154.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/ieee802154/af_802154.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/ieee802154/6lowpan.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/can
/lib/modules/3.10.98-yocto-standard/kernel/net/can/can.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/mac802154
/lib/modules/3.10.98-yocto-standard/kernel/net/mac802154/mac802154.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/netfilter
/lib/modules/3.10.98-yocto-standard/kernel/net/netfilter/xt_REDIRECT.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/netfilter/xt_u32.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/netfilter/xt_pkttype.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/netfilter/xt_mac.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/netfilter/xt_TCPMSS.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/netfilter/xt_multiport.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/netfilter/xt_connbytes.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/netfilter/xt_hashlimit.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/netfilter/xt_dccp.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/netfilter/xt_hl.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/netfilter/xt_string.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/netfilter/xt_dscp.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/netfilter/xt_realm.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/netfilter/xt_limit.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/netfilter/xt_NFLOG.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/netfilter/xt_HL.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/netfilter/xt_connmark.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/netfilter/xt_iprange.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/netfilter/xt_addrtype.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/netfilter/xt_conntrack.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/netfilter/xt_comment.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/netfilter/xt_physdev.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/netfilter/xt_ecn.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/netfilter/xt_helper.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/netfilter/xt_sctp.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/netfilter/xt_tcpudp.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/netfilter/xt_statistic.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/netfilter/x_tables.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/netfilter/xt_state.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/netfilter/xt_tcpmss.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/netfilter/xt_nat.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/netfilter/xt_policy.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/netfilter/nf_nat.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/netfilter/xt_NETMAP.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/netfilter/xt_length.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/netfilter/xt_TRACE.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/netfilter/xt_quota.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/netfilter/xt_mark.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/netfilter/xt_connlimit.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/mac80211
/lib/modules/3.10.98-yocto-standard/kernel/net/mac80211/mac80211.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/ipv6
/lib/modules/3.10.98-yocto-standard/kernel/net/ipv6/netfilter
/lib/modules/3.10.98-yocto-standard/kernel/net/ipv6/netfilter/ip6table_security.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/ipv6/netfilter/ip6table_filter.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/ipv6/netfilter/nf_conntrack_ipv6.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/ipv6/netfilter/ip6t_frag.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/ipv6/netfilter/ip6t_REJECT.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/ipv6/netfilter/ip6_tables.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/ipv6/netfilter/ip6t_rt.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/ipv6/netfilter/ip6t_hbh.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/ipv6/netfilter/ip6t_eui64.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/ipv6/netfilter/ip6t_rpfilter.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/ipv6/netfilter/ip6t_ipv6header.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/ipv6/netfilter/ip6t_ah.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/ipv6/netfilter/ip6table_mangle.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/ipv6/netfilter/ip6table_raw.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/ipv6/netfilter/nf_defrag_ipv6.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/ipv6/netfilter/ip6t_mh.ko
/lib/modules/3.10.98-yocto-standard/kernel/net/bridge
/lib/modules/3.10.98-yocto-standard/kernel/net/bridge/netfilter
/lib/modules/3.10.98-yocto-standard/kernel/net/bridge/netfilter/ebtables.ko
/lib/modules/3.10.98-yocto-standard/kernel/lib
/lib/modules/3.10.98-yocto-standard/kernel/lib/crc-itu-t.ko
/lib/modules/3.10.98-yocto-standard/kernel/lib/ts_bm.ko
/lib/modules/3.10.98-yocto-standard/kernel/lib/crc-ccitt.ko
/lib/modules/3.10.98-yocto-standard/kernel/lib/ts_kmp.ko
/lib/modules/3.10.98-yocto-standard/kernel/lib/ts_fsm.ko
/lib/modules/3.10.98-yocto-standard/kernel/fs
/lib/modules/3.10.98-yocto-standard/kernel/fs/ecryptfs
/lib/modules/3.10.98-yocto-standard/kernel/fs/ecryptfs/ecryptfs.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers
/lib/modules/3.10.98-yocto-standard/kernel/drivers/misc
/lib/modules/3.10.98-yocto-standard/kernel/drivers/misc/bcm-lpm
/lib/modules/3.10.98-yocto-standard/kernel/drivers/misc/bcm-lpm/bcm_bt_lpm.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/misc/bmp085-i2c.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/iio
/lib/modules/3.10.98-yocto-standard/kernel/drivers/iio/common
/lib/modules/3.10.98-yocto-standard/kernel/drivers/iio/common/st_sensors
/lib/modules/3.10.98-yocto-standard/kernel/drivers/iio/common/st_sensors/st_sensors_spi.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/iio/common/st_sensors/st_sensors.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/iio/common/st_sensors/st_sensors_i2c.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/iio/magnetometer
/lib/modules/3.10.98-yocto-standard/kernel/drivers/iio/magnetometer/st_magn.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/iio/magnetometer/ak8975.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/iio/magnetometer/st_magn_i2c.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/iio/magnetometer/st_magn_spi.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/iio/gyro
/lib/modules/3.10.98-yocto-standard/kernel/drivers/iio/gyro/st_gyro.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/iio/gyro/st_gyro_spi.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/iio/gyro/adis16136.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/iio/gyro/itg3200.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/iio/gyro/st_gyro_i2c.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/iio/light
/lib/modules/3.10.98-yocto-standard/kernel/drivers/iio/light/vcnl4000.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/iio/light/adjd_s311.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/iio/light/tsl2563.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/iio/accel
/lib/modules/3.10.98-yocto-standard/kernel/drivers/iio/accel/kxsd9.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/iio/accel/st_accel_i2c.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/iio/accel/st_accel_spi.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/iio/accel/st_accel.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/iio/adc
/lib/modules/3.10.98-yocto-standard/kernel/drivers/iio/adc/ad7887.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/iio/adc/ad7476.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/iio/adc/ad7923.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/iio/adc/ti-adc081c.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/iio/adc/ad_sigma_delta.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/iio/adc/ad7298.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/iio/adc/max1363.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/iio/adc/ad7793.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/iio/adc/ad7791.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/iio/adc/ad7266.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/iio/imu
/lib/modules/3.10.98-yocto-standard/kernel/drivers/iio/imu/adis_lib.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/iio/imu/inv_mpu6050
/lib/modules/3.10.98-yocto-standard/kernel/drivers/iio/imu/inv_mpu6050/inv-mpu6050.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/iio/imu/adis16400.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/iio/imu/adis16480.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/iio/dac
/lib/modules/3.10.98-yocto-standard/kernel/drivers/iio/dac/mcp4725.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/nfc
/lib/modules/3.10.98-yocto-standard/kernel/drivers/nfc/pn544
/lib/modules/3.10.98-yocto-standard/kernel/drivers/nfc/pn544/pn544.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/nfc/pn544/pn544_i2c.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/nfc/pn533.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/nfc/microread
/lib/modules/3.10.98-yocto-standard/kernel/drivers/nfc/microread/microread.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/nfc/microread/microread_i2c.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/usb
/lib/modules/3.10.98-yocto-standard/kernel/drivers/usb/serial
/lib/modules/3.10.98-yocto-standard/kernel/drivers/usb/serial/ipw.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/usb/serial/oti6858.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/usb/serial/ark3116.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/usb/serial/pl2303.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/usb/serial/option.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/usb/serial/ch341.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/usb/serial/usb_wwan.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/usb/serial/ftdi_sio.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/usb/serial/cp210x.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/usb/serial/belkin_sa.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/usb/serial/qcserial.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/usb/serial/ti_usb_3410_5052.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/usb/serial/f81232.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/usb/serial/spcp8x5.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/usb/serial/sierra.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/usb/gadget
/lib/modules/3.10.98-yocto-standard/kernel/drivers/usb/gadget/g_multi.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/usb/gadget/u_serial.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/usb/gadget/libcomposite.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/usb/gadget/usb_f_acm.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/net
/lib/modules/3.10.98-yocto-standard/kernel/drivers/net/usb
/lib/modules/3.10.98-yocto-standard/kernel/drivers/net/usb/usbnet.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/net/usb/dm9601.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/net/usb/mcs7830.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/net/usb/ax88179_178a.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/net/usb/r8152.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/net/usb/cdc_ncm.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/net/usb/smsc95xx.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/net/usb/rtl8150.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/net/usb/cdc_subset.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/net/usb/smsc75xx.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/net/usb/asix.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/net/usb/pegasus.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/net/can
/lib/modules/3.10.98-yocto-standard/kernel/drivers/net/can/slcan.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/net/can/vcan.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/hwmon
/lib/modules/3.10.98-yocto-standard/kernel/drivers/hwmon/lm75.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/media
/lib/modules/3.10.98-yocto-standard/kernel/drivers/media/v4l2-core
/lib/modules/3.10.98-yocto-standard/kernel/drivers/media/v4l2-core/videobuf2-memops.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/media/v4l2-core/videobuf2-vmalloc.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/media/v4l2-core/videobuf2-core.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/media/usb
/lib/modules/3.10.98-yocto-standard/kernel/drivers/media/usb/uvc
/lib/modules/3.10.98-yocto-standard/kernel/drivers/media/usb/uvc/uvcvideo.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/media/usb/gspca
/lib/modules/3.10.98-yocto-standard/kernel/drivers/media/usb/gspca/gspca_main.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/staging
/lib/modules/3.10.98-yocto-standard/kernel/drivers/staging/iio
/lib/modules/3.10.98-yocto-standard/kernel/drivers/staging/iio/magnetometer
/lib/modules/3.10.98-yocto-standard/kernel/drivers/staging/iio/magnetometer/hmc5843.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/staging/iio/light
/lib/modules/3.10.98-yocto-standard/kernel/drivers/staging/iio/light/isl29018.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/staging/iio/light/tsl2x7x_core.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/staging/iio/light/tsl2583.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/staging/iio/light/isl29028.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/staging/iio/accel
/lib/modules/3.10.98-yocto-standard/kernel/drivers/staging/iio/accel/lis3l02dq.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/staging/iio/trigger
/lib/modules/3.10.98-yocto-standard/kernel/drivers/staging/iio/trigger/iio-trig-sysfs.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/spi
/lib/modules/3.10.98-yocto-standard/kernel/drivers/spi/spidev.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/input
/lib/modules/3.10.98-yocto-standard/kernel/drivers/input/misc
/lib/modules/3.10.98-yocto-standard/kernel/drivers/input/misc/mpu3050.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/input/misc/adxl34x-i2c.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/input/misc/adxl34x.ko
/lib/modules/3.10.98-yocto-standard/kernel/drivers/input/misc/adxl34x-spi.ko
/lib/modules/3.10.98-yocto-standard/extra
/lib/modules/3.10.98-yocto-standard/extra/i2c-edison-mpu6050.ko
/lib/modules/3.10.98-yocto-standard/extra/bcm4334x.ko
/lib/modules/3.10.98-yocto-standard/modules.builtin.bin
/lib/modules/3.10.98-yocto-standard/modules.dep
/lib/modules/3.10.98-yocto-standard/modules.builtin
/lib/modules/3.10.98-yocto-standard/modules.dep.bin
/lib/modules/3.10.98-yocto-standard/modules.order
/lib/modules/3.10.98-yocto-standard/modules.symbols.bin
/lib/modules/3.10.98-yocto-standard/modules.devname
/lib/modules/3.10.98-yocto-standard/modules.alias
/lib/modules/3.10.98-yocto-standard/modules.softdep
root@edison:~# 
```