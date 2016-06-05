# WiFi

```sh
root@edison:~# connmanctl
connmanctl> enable wifi
Enabled wifi
connmanctl> scan wifi
Scan completed for wifi
connmanctl> services
                         wifi_784b87a53a73_hidden_managed_none
    INFINITUMfjph        wifi_784b87a53a73_494e46494e4954554d666a7068_managed_psk
    17057Abril           wifi_784b87a53a73_3137303537416272696c_managed_psk
    INFINITUM8240C7      wifi_784b87a53a73_494e46494e4954554d383234304337_managed_psk
    CACUNAT              wifi_784b87a53a73_434143554e4154_managed_wep
connmanctl> agent on
Agent registered
connmanctl> connect wifi_784b87a53a73_494e46494e4954554d666a7068_managed_psk
Agent RequestInput wifi_784b87a53a73_494e46494e4954554d666a7068_managed_psk
  Passphrase = [ Type=psk, Requirement=mandatory, Alternates=[ WPS ] ]
  WPS = [ Type=wpspin, Requirement=alternate ]
Passphrase? 
Connected wifi_784b87a53a73_494e46494e4954554d666a7068_managed_psk
connmanctl> exit
root@edison:~# ifconfig
lo        Link encap:Local Loopback  
          inet addr:127.0.0.1  Mask:255.0.0.0
          inet6 addr: ::1%3220015836/128 Scope:Host
          UP LOOPBACK RUNNING  MTU:65536  Metric:1
          RX packets:453 errors:0 dropped:0 overruns:0 frame:0
          TX packets:453 errors:0 dropped:0 overruns:0 carrier:0
          collisions:0 txqueuelen:0 
          RX bytes:32294 (31.5 KiB)  TX bytes:32294 (31.5 KiB)

wlan0     Link encap:Ethernet  HWaddr 78:4B:87:A5:3A:73  
          inet addr:192.168.1.69  Bcast:192.168.1.255  Mask:255.255.255.0
          inet6 addr: fe80::7a4b:87ff:fea5:3a73%3220015836/64 Scope:Link
          UP BROADCAST RUNNING MULTICAST  MTU:1500  Metric:1
          RX packets:24 errors:0 dropped:0 overruns:0 frame:0
          TX packets:48 errors:0 dropped:0 overruns:0 carrier:0
          collisions:0 txqueuelen:1000 
          RX bytes:3365 (3.2 KiB)  TX bytes:6236 (6.0 KiB)

root@edison:~# 
```
