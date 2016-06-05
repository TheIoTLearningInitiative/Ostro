# Boot Up

```sh
Linux kernel version 3.10.98-yocto-standard (jenkins@ostro-worker-20) #1 SMP PREEMPT Fri Apr 29 15:11:6
Building boot_params at 0x00090000
Loading bzImage at address 00100000 (5281264 bytes)
Magic signature found
Kernel command line: "rootwait root=PARTUUID=012b3303-34ac-284d-99b4-34e03a2335f4 rootfstype=ext4 cons"

Starting kernel ...

[    0.622458] tpm_tis tpm_tis: tpm_transmit: tpm_send: error -5
[    0.622537] tpm_tis tpm_tis: A TPM error (-5) occurred attempting to determine the timeouts
[    0.622641] tpm_tis tpm_tis: tpm_transmit: tpm_send: error -5
[    0.622703] tpm_tis tpm_tis: Could not get TPM timeouts and durations
[    1.562816] pmic_ccsm pmic_ccsm: Error reading battery profile from battid frmwrk
[    1.572425] pmic_ccsm pmic_ccsm: Battery Over heat exception
[    1.572502] pmic_ccsm pmic_ccsm: Battery0 temperature inside boundary

Welcome to Ostro OS 1.0~snapshot-20160502!

[  OK  ] Created slice User and Session Slice.
[  OK  ] Listening on /dev/initctl Compatibility Named Pipe.
[  OK  ] Created slice System Slice.
[  OK  ] Created slice system-getty.slice.
[  OK  ] Created slice system-wpa_supplicant.slice.
[  OK  ] Reached target Slices.
[  OK  ] Created slice system-serial\x2dgetty.slice.
[  OK  ] Started Dispatch Password Requests to Console Directory Watch.
[  OK  ] Listening on Journal Socket (/dev/log).
[  OK  ] Started Forward Password Requests to Wall Directory Watch.
[  OK  ] Listening on Journal Socket.
         Starting File System Check on Root Device...
         Starting ip6tables firewall...
         Mounting Temporary Directory...
         Starting iptables firewall...
         Starting Create list of required st... nodes for the current kernel...
         Starting Setup Virtual Console...
         Mounting Debug File System...
         Starting Load Kernel Modules...
[  OK  ] Listening on udev Kernel Socket.
[  OK  ] Listening on Network Service Netlink Socket.
[  OK  ] Reached target Swap.
         Starting Journal Service...
[  OK  ] Reached target Paths.
         Mounting POSIX Message Queue File System...
[  OK  ] Reached target Remote File Systems.
[  OK  ] Listening on udev Control Socket.
[  OK  ] Mounted Debug File System.
[  OK  ] Mounted POSIX Message Queue File System.
[  OK  ] Mounted Temporary Directory.
[  OK  ] Started File System Check on Root Device.
[  OK  ] Started ip6tables firewall.
[  OK  ] Started iptables firewall.
[  OK  ] Started Create list of required sta...ce nodes for the current kernel.
[  OK  ] Started Setup Virtual Console.
[  OK  ] Started Journal Service.
[  OK  ] Started Load Kernel Modules.
         Starting Apply Kernel Variables...
         Mounting FUSE Control File System...
         Mounting Configuration File System...
         Starting Remount Root and Kernel File Systems...
[  OK  ] Mounted FUSE Control File System.
[  OK  ] Mounted Configuration File System.
[  OK  ] Started Apply Kernel Variables.
[  OK  ] Started Remount Root and Kernel File Systems.
         Starting Create System Users...
         Starting Rebuild Dynamic Linker Cache...
         Starting Rebuild Hardware Database...
         Starting Flush Journal to Persistent Storage...
[  OK  ] Started Create System Users.
[  OK  ] Started Flush Journal to Persistent Storage.
[  OK  ] Started Rebuild Dynamic Linker Cache.
         Starting Create Static Device Nodes in /dev...
[  OK  ] Started Create Static Device Nodes in /dev.
         Starting udev Kernel Device Manager...
[  OK  ] Reached target Local File Systems (Pre).
         Mounting /var/volatile...
[  OK  ] Mounted /var/volatile.
[  OK  ] Started udev Kernel Device Manager.
[  OK  ] Found device /sys/subsystem/net/devices/wlan0.
         Starting Load/Save Random Seed...
[  OK  ] Started Load/Save Random Seed.
[  OK  ] Started Rebuild Hardware Database.
         Starting udev Coldplug all Devices...
[  OK  ] Started udev Coldplug all Devices.
[  OK  ] Found device /dev/ttyMFD2.
[  OK  ] Found device /dev/mmcblk0p5.
         Mounting /factory...
[  OK  ] Mounted /factory.
[  OK  ] Reached target Local File Systems.
         Starting Commit a transient machine-id on disk...
         Starting Rebuild Journal Catalog...
         Starting Create Volatile Files and Directories...
[  OK  ] Started Rebuild Journal Catalog.
[  OK  ] Started Create Volatile Files and Directories.
[  OK  ] Reached target Sound Card.
         Starting Network Time Synchronization...
         Starting Update UTMP about System Boot/Shutdown...
[  OK  ] Listening on Load/Save RF Kill Switch Status /dev/rfkill Watch.
         Starting Update is Completed...
         Starting Load/Save RF Kill Switch Status...
[  OK  ] Started Commit a transient machine-id on disk.
[  OK  ] Started Update is Completed.
[  OK  ] Started Load/Save RF Kill Switch Status.
[  OK  ] Started Network Time Synchronization.
[  OK  ] Started Update UTMP about System Boot/Shutdown.
[  OK  ] Reached target System Time Synchronized.
[  OK  ] Reached target System Initialization.
         Starting sshd.socket.
[  OK  ] Started Daily Cleanup of Temporary Directories.
[  OK  ] Reached target Timers.
[  OK  ] Listening on D-Bus System Message Bus Socket.
[  OK  ] Listening on sshd.socket.
[  OK  ] Reached target Sockets.
[  OK  ] Reached target Basic System.
[  OK  ] Started Bluetooth rf kill event daemon.
         Starting Permit User Sessions...
[  OK  ] Started D-Bus System Message Bus.
         Starting Connection service...
         Starting Network Service...
         Starting Login Service...
[  OK  ] Started WPA supplicant daemon (interface-specific version).
[  OK  ] Started Daemon to load edison mcu app binary.
Application available at (physical) address 0x04819000
        VRL mapped to 0xff213000
        App size = 11508 bytes

        App Authentication feature is disabled!
        Resetting I������2j��ٲy to receive application *** 
[  OK    OK  ] Started Permit User Sessions.
[  OK  ] Started Connection service.
[  OK  ] Started Login Service.
[  OK  ] Started Getty on tty1.
[  OK  ] Started Serial Getty on ttyMFD2.
[  OK  ] Reached target Login Prompts.
[  OK  ] Reached target Network.
[  OK  ] Reached target Multi-User System.
         Starting Update UTMP about System Runlevel Changes...
[  OK  ] Started Update UTMP about System Runlevel Changes.

Ostro OS 1.0~snapshot-20160428 edison ttyMFD2

edison login: root (automatic login)

Last login: Thu Apr 28 00:41:36 UTC 2016 on tty1
************************************
*** This is a development image! ***
*** Do not use in production.    ***
************************************
root@edison:~# 
```

```sh
root@edison:~# uname -a 
Linux edison 3.10.98-yocto-standard #1 SMP PREEMPT Fri Apr 29 15:11:11 UTC 2016 i686 GNU/Linux
root@edison:~# 
```

[Configuring an IP Address in the Ostro™ OS](https://ostroproject.org/documentation/howtos/ip-address-config.html)

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
```

```sh
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

```sh
root@edison:~# ping google.com
PING google.com (216.58.193.46): 56 data bytes
64 bytes from 216.58.193.46: seq=0 ttl=58 time=445.769 ms
64 bytes from 216.58.193.46: seq=1 ttl=58 time=932.851 ms
64 bytes from 216.58.193.46: seq=2 ttl=58 time=1467.134 ms
^C
--- google.com ping statistics ---
4 packets transmitted, 3 packets received, 25% packet loss
round-trip min/avg/max = 445.769/948.584/1467.134 ms
root@edison:~# 
```

```sh
root@edison:~# iptables-save > /home/root/firewall.rules
root@edison:~# iptables -F
root@edison:~# iptables -X
root@edison:~# iptables -t nat -F
root@edison:~# iptables -t nat -X
root@edison:~# iptables -t mangle -F
root@edison:~# iptables -t mangle -X
root@edison:~# iptables -P INPUT ACCEPT
root@edison:~# iptables -P OUTPUT ACCEPT     
root@edison:~# iptables -P FORWARD ACCEPT    
```