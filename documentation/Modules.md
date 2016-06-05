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