# Power

```sh
root@edison:~# echo mem > /sys/power/state 
[   54.155296] intel_scu_watchdog_evo: watchdog_stop
[   54.197155] pci_pm_suspend(): sdhci_pci_suspend+0x0/0xd0 returns -16
[   54.197171] dpm_run_callback(): pci_pm_suspend+0x0/0x1b0 returns -16
[   54.197183] PM: Device 0000:00:01.3 failed to suspend async: error -16
[   54.228708] PM: Some devices failed to suspend
-sh: echo: write error: Device or resource busy
root@edison:~# 
```