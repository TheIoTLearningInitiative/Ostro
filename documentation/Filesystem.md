# Filesystem

```sh
root@edison:~# cd /
root@edison:/# ls
bin         dev         factory     lib         media       proc        sbin        sys         usr
boot        etc         home        lost+found  mnt         run         srv         tmp         var
root@edison:/# ls /home/
root
root@edison:/# 
```

```sh
root@edison:~# df -h
Filesystem                Size      Used Available Use% Mounted on
/dev/root                 1.8G    322.2M      1.4G  19% /
devtmpfs                480.0M         0    480.0M   0% /dev
tmpfs                   480.3M         0    480.3M   0% /dev/shm
tmpfs                   480.3M     12.5M    467.8M   3% /run
tmpfs                   480.3M         0    480.3M   0% /sys/fs/cgroup
tmpfs                   480.3M         0    480.3M   0% /tmp
tmpfs                   480.3M      8.0K    480.3M   0% /var/volatile
/dev/mmcblk0p5         1003.0K     19.0K    913.0K   2% /factory
tmpfs                    96.1M         0     96.1M   0% /run/user/0
root@edison:~# 
```

```sh
root@edison:~# df -h                                                                                   
Filesystem                Size      Used Available Use% Mounted on
/dev/root                 1.8G      1.1G    606.9M  65% /
devtmpfs                480.0M         0    480.0M   0% /dev
tmpfs                   480.3M         0    480.3M   0% /dev/shm
tmpfs                   480.3M     12.5M    467.7M   3% /run
tmpfs                   480.3M         0    480.3M   0% /sys/fs/cgroup
tmpfs                   480.3M         0    480.3M   0% /tmp                                 
tmpfs                   480.3M      8.0K    480.3M   0% /var/volatile
/dev/mmcblk0p5         1003.0K     19.0K    913.0K   2% /factory
tmpfs                    96.1M         0     96.1M   0% /run/user/0
root@edison:~# 
```

```sh
root@edison:~# mount
/dev/mmcblk0p8 on / type ext4 (rw,nodev,noatime,discard,noauto_da_alloc,i_version,data=ordered)
devtmpfs on /dev type devtmpfs (rw,relatime,size=491528k,nr_inodes=122882,mode=755)
sysfs on /sys type sysfs (rw,nosuid,nodev,noexec,relatime)
proc on /proc type proc (rw,relatime)
securityfs on /sys/kernel/security type securityfs (rw,nosuid,nodev,noexec,relatime)
smackfs on /sys/fs/smackfs type smackfs (rw,nosuid,nodev,noexec,relatime)
tmpfs on /dev/shm type tmpfs (rw,nosuid,nodev)
devpts on /dev/pts type devpts (rw,relatime,gid=5,mode=620,ptmxmode=000)
tmpfs on /run type tmpfs (rw,nosuid,nodev,mode=755)
tmpfs on /sys/fs/cgroup type tmpfs (ro,nosuid,nodev,noexec,mode=755)
cgroup on /sys/fs/cgroup/systemd type cgroup (rw,nosuid,nodev,noexec,relatime,xattr,release_agent=/lib)
pstore on /sys/fs/pstore type pstore (rw,nosuid,nodev,noexec,relatime)
cgroup on /sys/fs/cgroup/freezer type cgroup (rw,nosuid,nodev,noexec,relatime,freezer)
cgroup on /sys/fs/cgroup/cpuset type cgroup (rw,nosuid,nodev,noexec,relatime,cpuset)
cgroup on /sys/fs/cgroup/devices type cgroup (rw,nosuid,nodev,noexec,relatime,devices)
cgroup on /sys/fs/cgroup/cpu,cpuacct type cgroup (rw,nosuid,nodev,noexec,relatime,cpuacct,cpu)
cgroup on /sys/fs/cgroup/perf_event type cgroup (rw,nosuid,nodev,noexec,relatime,perf_event)
cgroup on /sys/fs/cgroup/blkio type cgroup (rw,nosuid,nodev,noexec,relatime,blkio)
tmpfs on /tmp type tmpfs (rw,relatime)
debugfs on /sys/kernel/debug type debugfs (rw,relatime)
mqueue on /dev/mqueue type mqueue (rw,relatime)
fusectl on /sys/fs/fuse/connections type fusectl (rw,relatime)
configfs on /sys/kernel/config type configfs (rw,relatime)
tmpfs on /var/volatile type tmpfs (rw,relatime)
/dev/mmcblk0p5 on /factory type ext4 (ro,noatime)
tmpfs on /run/user/0 type tmpfs (rw,nosuid,nodev,relatime,size=98360k,mode=700)
root@edison:~# 
```