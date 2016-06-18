# Services

```sh
root@edison:~# ls /lib/systemd/system
-.slice                                 shutdown.target
atop.service                            sigpwr.target
autovt@.service                         sleep.target
basic.target                            slices.target
bluetooth-rfkill-event.service          smartcard.target
bluetooth.service                       sockets.target
bluetooth.target                        sockets.target.wants
busnames.target                         sound.target
busnames.target.wants                   sshd.socket
connman.service                         sshd.socket.d
console-getty.service                   sshd@.service
console-shell.service                   sshdgenkeys.service
container-getty@.service                suspend.target
ctrl-alt-del.target                     swap.target
dbus-org.freedesktop.hostname1.service  sys-fs-fuse-connections.mount
dbus-org.freedesktop.locale1.service    sys-kernel-config.mount
dbus-org.freedesktop.login1.service     sys-kernel-debug.mount
dbus-org.freedesktop.machine1.service   sysinit.target
dbus-org.freedesktop.network1.service   sysinit.target.wants
dbus-org.freedesktop.timedate1.service  syslog.socket
dbus.service                            system-update.target
dbus.socket                             system.slice
dbus.target.wants                       systemd-ask-password-console.path
debug-shell.service                     systemd-ask-password-console.service
default.target                          systemd-ask-password-wall.path
dev-hugepages.mount                     systemd-ask-password-wall.service
dev-mqueue.mount                        systemd-backlight@.service
emergency.service                       systemd-bootchart.service
emergency.target                        systemd-exit.service
exit.target                             systemd-fsck-root.service
final.target                            systemd-fsck@.service
getty.target                            systemd-halt.service
getty@.service                          systemd-hibernate-resume@.service
graphical.target                        systemd-hibernate.service
graphical.target.wants                  systemd-hostnamed.service
halt-local.service                      systemd-hwdb-update.service
halt.target                             systemd-hybrid-sleep.service
hibernate.target                        systemd-initctl.service
hybrid-sleep.target                     systemd-initctl.socket
initrd-cleanup.service                  systemd-journal-catalog-update.service
initrd-fs.target                        systemd-journal-flush.service
initrd-parse-etc.service                systemd-journald-audit.socket
initrd-root-fs.target                   systemd-journald-dev-log.socket
initrd-switch-root.service              systemd-journald.service
initrd-switch-root.target               systemd-journald.service.d
initrd-udevadm-cleanup-db.service       systemd-journald.socket
initrd.target                           systemd-kexec.service
ip6tables.service                       systemd-localed.service
iptables.service                        systemd-logind.service
kexec.target                            systemd-machine-id-commit.service
kmod-static-nodes.service               systemd-machine-id-commit.service.d
ldconfig.service                        systemd-machined.service
local-fs-pre.target                     systemd-modules-load.service
local-fs.target                         systemd-networkd-wait-online.service
local-fs.target.wants                   systemd-networkd.service
machine.slice                           systemd-networkd.socket
machines.target                         systemd-nspawn@.service
mcu_fw_loader.service                   systemd-poweroff.service
multi-user.target                       systemd-quotacheck.service
multi-user.target.wants                 systemd-random-seed.service
network-online.target                   systemd-random-seed.service.d
network-pre.target                      systemd-reboot.service
network.target                          systemd-remount-fs.service
nss-lookup.target                       systemd-rfkill.service
nss-user-lookup.target                  systemd-rfkill.socket
org.freedesktop.hostname1.busname       systemd-suspend.service
org.freedesktop.locale1.busname         systemd-sysctl.service
org.freedesktop.login1.busname          systemd-sysusers.service
org.freedesktop.machine1.busname        systemd-timedated.service
org.freedesktop.network1.busname        systemd-timesyncd.service
org.freedesktop.systemd1.busname        systemd-tmpfiles-clean.service
org.freedesktop.timedate1.busname       systemd-tmpfiles-clean.timer
paths.target                            systemd-tmpfiles-setup-dev.service
poweroff.target                         systemd-tmpfiles-setup.service
poweroff.target.wants                   systemd-tmpfiles-setup.service.d
printer.target                          systemd-udev-settle.service
quotaon.service                         systemd-udev-trigger.service
rc-local.service                        systemd-udevd-control.socket
reboot.target                           systemd-udevd-kernel.socket
reboot.target.wants                     systemd-udevd.service
remote-fs-pre.target                    systemd-update-done.service
remote-fs.target                        systemd-update-utmp-runlevel.service
rescue.service                          systemd-update-utmp.service
rescue.target                           systemd-user-sessions.service
rescue.target.wants                     systemd-vconsole-setup.service
rpcbind.target                          time-sync.target
run-postinsts.service                   timers.target
runlevel0.target                        timers.target.wants
runlevel1.target                        tmp.mount
runlevel1.target.wants                  tmp.mount.d
runlevel2.target                        umount.target
runlevel2.target.wants                  user.slice
runlevel3.target                        user@.service
runlevel3.target.wants                  var-lib-machines.mount
runlevel4.target                        var-volatile-lib.service
runlevel4.target.wants                  wpa_supplicant-nl80211@.service
runlevel5.target                        wpa_supplicant-wired@.service
runlevel5.target.wants                  wpa_supplicant.service
runlevel6.target                        wpa_supplicant@.service
serial-getty@.service
root@edison:~# 
```

```sh
root@edison:~# systemctl stop iptables.service
root@edison:~# systemctl start iptables.service
root@edison:~# systemctl status iptables.service
```

```sh

```