# Reboot

```sh
root@edison:~# reboot
[  OK  ] Stopped target Timers.
[  OK  ] Stopped target Network.
         Stopping User Manager for UID 0...
[ 2580.551308] recv IRQ when we are not startup yet
         Stopping Session c2 of user root.
[  OK  ] Stopped target Multi-User System.
[  OK  ] Stopped target Login Prompts.
         Stopping Network Service...
         Stopping Connection service...
[  OK  ] Removed slice system-wpa_supplicant.slice.
[  OK  ] Stopped target System Time Synchronized.
         Stopping Bluetooth rf kill event daemon...
         Stopping Serial Getty on ttyMFD2...
[  OK  ] Closed Load/Save RF Kill Switch Status /dev/rfkill Watch.
         Stopping Getty on tty1...
[  OK  ] Stopped Daily Cleanup of Temporary Directories.
[  OK  ] Stopped Session c1 of user root.
[  OK  ] Stopped target Sound Card.
         Stopping WPA supplicant...
[  OK  ] Stopped Bluetooth rf kill event daemon.
[  OK  ] Stopped Connection service.
[  OK  ] Stopped Network Service.
[  OK  ] Stopped Getty on tty1.
[  OK  ] Stopped Serial Getty on ttyMFD2.
[  OK  ] Stopped User Manager for UID 0.
[  OK  ] Stopped WPA supplicant.
[  OK  ] Stopped Session c2 of user root.
[  OK  ] Removed slice User Slice of root.
         Stopping Login Service...
[  OK  ] Removed slice system-serial\x2dgetty.slice.
[  OK  ] Removed slice system-getty.slice.
         Stopping Permit User Sessions...
         Stopping D-Bus System Message Bus...
[  OK  ] Stopped D-Bus System Message Bus.
[  OK  ] Stopped Login Service.
[  OK  ] Stopped Permit User Sessions.
[  OK  ] Stopped target Remote File Systems.
[  OK  ] Stopped target Basic System.
[  OK  ] Stopped target Slices.
[  OK  ] Removed slice User and Session Slice.
[  OK  ] Stopped target Sockets.
         Stopping sshd.socket.
[  OK  ] Stopped target Paths.
[  OK  ] Stopped Dispatch Password Requests to Console Directory Watch.
[  OK  ] Stopped Forward Password Requests to Wall Directory Watch.
[  OK  ] Closed D-Bus System Message Bus Socket.
[  OK  ] Closed sshd.socket.
[  OK  ] Stopped iptables firewall.
[  OK  ] Stopped target System Initialization.
[  OK  ] Stopped Setup Virtual Console.
[  OK  ] Stopped Commit a transient machine-id on disk.
         Stopping Load/Save Random Seed...
[  OK  ] Stopped target Swap.
[  OK  ] Stopped Update is Completed.
[  OK  ] Stopped Rebuild Dynamic Linker Cache.
[  OK  ] Stopped Rebuild Hardware Database.
[  OK  ] Stopped Apply Kernel Variables.
[  OK  ] Stopped Load Kernel Modules.
         Stopping Network Time Synchronization...
[  OK  ] Stopped Rebuild Journal Catalog.
[  OK  ] Stopped ip6tables firewall.
[  OK  ] Stopped Network Time Synchronization.
[  OK  ] Stopped Load/Save Random Seed.
[  OK  ] Stopped Create Volatile Files and Directories.
[  OK  ] Stopped target Local File Systems.
         Unmounting /var/volatile...
         Unmounting /factory...
         Unmounting Temporary Directory...
         Unmounting /run/user/0...
[  OK  ] Unmounted /var/volatile.
[  OK  ] Unmounted /factory.
[  OK  ] Unmounted Temporary Directory.
[  OK  ] Unmounted /run/user/0.
[  OK  ] Reached target Unmount All Filesystems.
[  OK  ] Stopped target Local File Systems (Pre).
[  OK  ] Stopped Create Static Device Nodes in /dev.
[  OK  ] Stopped Create System Users.
[  OK  ] Stopped Remount Root and Kernel File Systems.
[  OK  ] Reached target Shutdown.
```
