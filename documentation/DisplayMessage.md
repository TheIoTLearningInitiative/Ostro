# Display Message

```sh
root@edison:~# dmesg
[    0.000000] Initializing cgroup subsys cpuset
[    0.000000] Initializing cgroup subsys cpu
[    0.000000] Initializing cgroup subsys cpuacct
[    0.000000] Linux version 3.10.98-yocto-standard (jenkins@ostro-worker-20) (gcc version 5.3.0 (GCC)6
[    0.000000] e820: BIOS-provided physical RAM map:
[    0.000000] BIOS-e820: [mem 0x0000000000000000-0x0000000000097fff] usable
[    0.000000] BIOS-e820: [mem 0x0000000000100000-0x0000000003ffffff] usable
[    0.000000] BIOS-e820: [mem 0x0000000004000000-0x0000000005ffffff] reserved
[    0.000000] BIOS-e820: [mem 0x0000000006000000-0x000000003f4fffff] usable
[    0.000000] BIOS-e820: [mem 0x000000003f500000-0x000000003fffffff] reserved
[    0.000000] BIOS-e820: [mem 0x00000000fec00000-0x00000000fec00fff] reserved
[    0.000000] BIOS-e820: [mem 0x00000000fec04000-0x00000000fec07fff] reserved
[    0.000000] BIOS-e820: [mem 0x00000000fee00000-0x00000000fee00fff] reserved
[    0.000000] BIOS-e820: [mem 0x00000000ff000000-0x00000000ffffffff] reserved
[    0.000000] NX (Execute Disable) protection: active
[    0.000000] SMBIOS 2.6 present.
[    0.000000] DMI: Intel Corporation Merrifield/BODEGA BAY, BIOS 466 2014.06.23:19.20.05
[    0.000000] e820: update [mem 0x00000000-0x00000fff] usable ==> reserved
[    0.000000] e820: remove [mem 0x000a0000-0x000fffff] usable
[    0.000000] e820: last_pfn = 0x3f500 max_arch_pfn = 0x1000000
[    0.000000] MTRR default type: uncachable
[    0.000000] MTRR fixed ranges enabled:
[    0.000000]   00000-9FFFF write-back
[    0.000000]   A0000-BFFFF uncachable
[    0.000000]   C0000-FFFFF write-back
[    0.000000] MTRR variable ranges enabled:
[    0.000000]   0 base 000000000 mask FC0000000 write-back
[    0.000000]   1 base 03F600000 mask FFFE00000 uncachable
[    0.000000]   2 base 03F800000 mask FFF800000 uncachable
[    0.000000]   3 base 004000000 mask FFE000000 uncachable
[    0.000000]   4 disabled
[    0.000000]   5 disabled
[    0.000000]   6 disabled
[    0.000000]   7 disabled
[    0.000000] x86 PAT enabled: cpu 0, old 0x7040600070406, new 0x7010600070106
[    0.000000] original variable MTRRs
[    0.000000] reg 0, base: 0GB, range: 1GB, type WB
[    0.000000] reg 1, base: 1014MB, range: 2MB, type UC
[    0.000000] reg 2, base: 1016MB, range: 8MB, type UC
[    0.000000] reg 3, base: 64MB, range: 32MB, type UC
[    0.000000] total RAM covered: 982M
[    0.000000] Found optimal setting for mtrr clean up
[    0.000000]  gran_size: 64K  chunk_size: 512M        num_reg: 5      lose cover RAM: 0G
[    0.000000] New variable MTRRs
[    0.000000] reg 0, base: 0GB, range: 512MB, type WB
[    0.000000] reg 1, base: 64MB, range: 32MB, type UC
[    0.000000] reg 2, base: 512MB, range: 512MB, type WB
[    0.000000] reg 3, base: 1014MB, range: 2MB, type UC
[    0.000000] reg 4, base: 1016MB, range: 8MB, type UC
[    0.000000] e820: update [mem 0x04000000-0x05ffffff] usable ==> reserved
[    0.000000] initial memory mapped: [mem 0x00000000-0x021fffff]
[    0.000000] Base memory trampoline at [c0094000] 94000 size 16384
[    0.000000] init_memory_mapping: [mem 0x00000000-0x000fffff]
[    0.000000]  [mem 0x00000000-0x000fffff] page 4k
[    0.000000] init_memory_mapping: [mem 0x37400000-0x375fffff]
[    0.000000]  [mem 0x37400000-0x375fffff] page 2M
[    0.000000] init_memory_mapping: [mem 0x34000000-0x373fffff]
[    0.000000]  [mem 0x34000000-0x373fffff] page 2M
[    0.000000] init_memory_mapping: [mem 0x00100000-0x03ffffff]
[    0.000000]  [mem 0x00100000-0x001fffff] page 4k
[    0.000000]  [mem 0x00200000-0x03ffffff] page 2M
[    0.000000] init_memory_mapping: [mem 0x06000000-0x33ffffff]
[    0.000000]  [mem 0x06000000-0x33ffffff] page 2M
[    0.000000] init_memory_mapping: [mem 0x37600000-0x377fdfff]
[    0.000000]  [mem 0x37600000-0x377fdfff] page 4k
[    0.000000] BRK [0x01dad000, 0x01dadfff] PGTABLE
[    0.000000] BRK [0x01dae000, 0x01daefff] PGTABLE
[    0.000000] 125MB HIGHMEM available.
[    0.000000] 887MB LOWMEM available.
[    0.000000]   mapped low ram: 0 - 377fe000
[    0.000000]   low ram: 0 - 377fe000
[    0.000000] BRK [0x01daf000, 0x01daffff] PGTABLE
[    0.000000] Zone ranges:
[    0.000000]   DMA      [mem 0x00001000-0x00ffffff]
[    0.000000]   Normal   [mem 0x01000000-0x377fdfff]
[    0.000000]   HighMem  [mem 0x377fe000-0x3f4fffff]
[    0.000000] Movable zone start for each node
[    0.000000] Early memory node ranges
[    0.000000]   node   0: [mem 0x00001000-0x00097fff]
[    0.000000]   node   0: [mem 0x00100000-0x03ffffff]
[    0.000000]   node   0: [mem 0x06000000-0x3f4fffff]
[    0.000000] On node 0 totalpages: 251031
[    0.000000] free_area_init_node: node 0, pgdat c1c038c0, node_mem_map f700e020
[    0.000000]   DMA zone: 32 pages used for memmap
[    0.000000]   DMA zone: 0 pages reserved
[    0.000000]   DMA zone: 3991 pages, LIFO batch:0
[    0.000000]   Normal zone: 1744 pages used for memmap
[    0.000000]   Normal zone: 215038 pages, LIFO batch:31
[    0.000000]   HighMem zone: 251 pages used for memmap
[    0.000000]   HighMem zone: 32002 pages, LIFO batch:7
[    0.000000] Using APIC driver default
[    0.000000] SFI: Simple Firmware Interface v0.81 http://simplefirmware.org
[    0.000000] SFI: SYST E61F0, 0060 (v1  INTEL INTELFDK)
[    0.000000] SFI: CPUS E6296, 0020 (v1  INTEL INTELFDK)
[    0.000000] SFI: FREQ E62C2, 0030 (v1  INTEL INTELFDK)
[    0.000000] SFI: MMAP E62FE, 01A4 (v1  INTEL INTELFDK)
[    0.000000] SFI: XSDT E64B0, 002C (v1  INTEL INTELFDK)
[    0.000000] SFI: APIC E653E, 0020 (v1  INTEL INTELFDK)
[    0.000000] SFI: WAKE E656A, 0020 (v2  INTEL INTELFDK)
[    0.000000] SFI: DEVS E659E, 044B (v1  INTEL INTELFDK)
[    0.000000] SFI: GPIO E69F5, 0964 (v1  INTEL INTELFDK)
[    0.000000] SFI: OEMB E7365, 0060 (v5 UMGFDK CFGINFO!)
[    0.000000] SFI: registering lapic[0]
[    0.000000] SFI: registering lapic[2]
[    0.000000] IOAPIC[0]: apic_id 0, version 32, address 0xfec00000, GSI 0-54
[    0.000000] smpboot: Allowing 2 CPUs, 0 hotplug CPUs
[    0.000000] nr_irqs_gsi: 71
[    0.000000] e820: [mem 0x40000000-0xfebfffff] available for PCI devices
[    0.000000] setup_percpu: NR_CPUS:2 nr_cpumask_bits:2 nr_cpu_ids:2 nr_node_ids:1
[    0.000000] PERCPU: Embedded 13 pages/cpu @f6fee000 s31808 r0 d21440 u53248
[    0.000000] pcpu-alloc: s31808 r0 d21440 u53248 alloc=13*4096
[    0.000000] pcpu-alloc: [0] 0 [0] 1 
[    0.000000] Built 1 zonelists in Zone order, mobility grouping on.  Total pages: 249255
[    0.000000] Kernel command line: rootwait root=PARTUUID=012b3303-34ac-284d-99b4-34e03a2335f4 rootfsp
[    0.000000] PID hash table entries: 4096 (order: 2, 16384 bytes)
[    0.000000] Dentry cache hash table entries: 131072 (order: 7, 524288 bytes)
[    0.000000] Inode-cache hash table entries: 65536 (order: 6, 262144 bytes)
[    0.000000] Initializing CPU#0
[    0.000000] Initializing HighMem for node 0 (000377fe:0003f500)
[    0.000000] Memory: 983028k/1037312k available (6929k kernel code, 21096k reserved, 3454k data, 512)
[    0.000000] virtual kernel memory layout:
                   fixmap  : 0xfff8b000 - 0xfffff000   ( 464 kB)
                   pkmap   : 0xff800000 - 0xffa00000   (2048 kB)
                   vmalloc : 0xf7ffe000 - 0xff7fe000   ( 120 MB)
                   lowmem  : 0xc0000000 - 0xf77fe000   ( 887 MB)
                     .init : 0xc1c25000 - 0xc1ca5000   ( 512 kB)
                     .data : 0xc18c46a0 - 0xc1c24280   (3454 kB)
                     .text : 0xc1200000 - 0xc18c46a0   (6929 kB)
[    0.000000] Checking if this processor honours the WP bit even in supervisor mode...Ok.
[    0.000000] SLUB: HWalign=64, Order=0-3, MinObjects=0, CPUs=2, Nodes=1
[    0.000000] Preemptible hierarchical RCU implementation.
[    0.000000]  Additional per-CPU info printed with stalls.
[    0.000000] NR_IRQS:2304 nr_irqs:512 16
[    0.000000] CPU 0 irqstacks, hard=f6808000 soft=f680a000
[    0.000000] Console: colour dummy device 80x25
[    0.000000] tsc: Detected 499.200 MHz processor
[    0.000008] Calibrating delay loop (skipped), value calculated using timer frequency.. 998.40 BogoM)
[    0.000031] pid_max: default: 32768 minimum: 301
[    0.000178] Security Framework initialized
[    0.000226] Smack:  Initializing.
[    0.000250] Yama: becoming mindful.
[    0.000323] Mount-cache hash table entries: 512
[    0.001279] Initializing cgroup subsys devices
[    0.001300] Initializing cgroup subsys freezer
[    0.001314] Initializing cgroup subsys blkio
[    0.001326] Initializing cgroup subsys perf_event
[    0.001439] CPU: Physical Processor ID: 0
[    0.001453] CPU: Processor Core ID: 0
[    0.001470] ENERGY_PERF_BIAS: Set to 'normal', was 'performance'
               ENERGY_PERF_BIAS: View and update with x86_energy_perf_policy(8)
[    0.001489] mce: CPU supports 6 MCE banks
[    0.001518] CPU0: Thermal monitoring enabled (TM1)
[    0.001558] Last level iTLB entries: 4KB 0, 2MB 0, 4MB 0
               Last level dTLB entries: 4KB 128, 2MB 0, 4MB 0
               tlb_flushall_shift: 6
[    0.001989] Freeing SMP alternatives: 28k freed
[    0.002042] SFI: MCFG E64F6, 003C (v1  INTEL INTELFDK)
[    0.002060] ftrace: allocating 27254 entries in 54 pages
[    0.066272] Enabling APIC mode:  Flat.  Using 1 I/O APICs
[    0.066329] smpboot: CPU0: Genuine Intel(R) CPU   4000  @  500MHz (fam: 06, model: 4a, stepping: 08)
[    0.066374] TSC deadline timer enabled
[    0.066434] Performance Events: no PEBS fmt2+, generic architected perfmon, Intel PMU driver.
[    0.066477] ... version:                3
[    0.066491] ... bit width:              40
[    0.066502] ... generic registers:      2
[    0.066514] ... value mask:             000000ffffffffff
[    0.066526] ... max period:             000000007fffffff
[    0.066537] ... fixed-purpose events:   3
[    0.066549] ... event mask:             0000000700000003
[    0.106839] ftrace: Allocated trace_printk buffers
[    0.157649] CPU 1 irqstacks, hard=f6b8c000 soft=f6b8e000
[    0.157670] smpboot: Booting Node   0, Processors  #1 OK
[    0.167873] Initializing CPU#1
[    0.168838] Skipped synchronization checks as TSC is reliable.
[    0.169220] NMI watchdog: enabled on all CPUs, permanently consumes one hw-PMU counter.
[    0.169296] Brought up 2 CPUs
[    0.169316] smpboot: Total of 2 processors activated (1996.80 BogoMIPS)
[    0.171038] devtmpfs: initialized
[    0.181097] SFI: SFI sysfs interfaces init success
[    0.181548] regulator-dummy: no parameters
[    0.181918] NET: Registered protocol family 16
[    0.183882] SFI OEMB Layout
[    0.183919]  OEMB signature               : OEMB
                OEMB length                  : 96
                OEMB revision                : 5
                OEMB checksum                : 0x9D
                OEMB oem_id                  : UMGFDK
                OEMB oem_table_id            : CFGINFO!
                OEMB board_id                : 0x02
                OEMB iafw version            : 002.001
                OEMB val_hooks version       : 002.001
                OEMB ia suppfw version       : 000.000
                OEMB scu runtime version     : 176.073
                OEMB ifwi version            : 237.013
[    0.184014] intel_soc_thermal: IPC bus = 0, name =         soc_thrm, irq = 0x 1
[    0.184172] IPC bus, name =        bcove_adc, irq = 0x32
[    0.184322] IPC bus, name =       bcove_thrm, irq = 0x34
[    0.184487] IPC bus, name =  bcove_power_btn, irq = 0x1e
[    0.184616] IPC bus, name =        pmic_ccsm, irq = 0x1b
[    0.184798] SDIO bus = 1, name = bcm43xx_clk_vmmc, ref_clock = 26000000, addr =0x401
[    0.184813] Using generic wifi platform data
[    0.184828] wifi_platform_data: GPIO == 64
[    0.184927] IPC bus, name =        msic_gpio, irq = 0x31
[    0.185075] I2C bus = 1, name =      pcal9555a-1, irq = 0x 0, addr = 0x20
[    0.185109] I2C bus = 1, name =      pcal9555a-2, irq = 0x 0, addr = 0x21
[    0.185139] I2C bus = 1, name =      pcal9555a-3, irq = 0x 0, addr = 0x22
[    0.185170] I2C bus = 1, name =      pcal9555a-4, irq = 0x 0, addr = 0x23
[    0.185201] SPI bus=5, name=         ads7955, irq=0x 0, max_freq=20000000, cs=0
[    0.185220] SPI bus=5, name=          spidev, irq=0x 0, max_freq=25000000, cs=1
[    0.185265] pgrr = 000003d5
[    0.185630] PCI: MMCONFIG for domain 0000 [bus 00-00] at [mem 0x3f500000-0x3f5fffff] (base 0x3f5000)
[    0.185653] PCI: MMCONFIG at [mem 0x3f500000-0x3f5fffff] reserved in E820
[    0.185665] PCI: Using MMCONFIG for extended config space
[    0.185678] PCI: Using configuration type 1 for base access
[    0.195546] bio: create slab <bio-0> at 0
[    0.196791] vgaarb: loaded
[    0.197297] SCSI subsystem initialized
[    0.197562] usbcore: registered new interface driver usbfs
[    0.197647] usbcore: registered new interface driver hub
[    0.197827] usbcore: registered new device driver usb
[    0.198073] media: Linux media interface: v0.10
[    0.198144] Linux video capture interface: v2.00
[    0.198202] pps_core: LinuxPPS API ver. 1 registered
[    0.198217] pps_core: Software ver. 5.3.6 - Copyright 2005-2007 Rodolfo Giometti <giometti@linux.it>
[    0.198249] PTP clock support registered
[    0.198612]  remoteproc0: intel_rproc_scu is available
[    0.198632]  remoteproc0: Note: remoteproc is still under development and considered experimental.
[    0.198647]  remoteproc0: THE BINARY FORMAT IS NOT YET FINALIZED, and backward compatibility isn't .
[    0.199004]  remoteproc0: registered virtio0 (type 7)
[    0.199216]  remoteproc0: powering up intel_rproc_scu
[    0.199243]  remoteproc0: Booting fw image intel_mid/intel_mid_remoteproc.fw, size 4456
[    0.199281] Started intel scu remote processor
[    0.199297]  remoteproc0: remote processor intel_rproc_scu is now up
[    0.199620] virtio_rpmsg_bus virtio0: creating channel rpmsg_bcove_adc addr 0x24
[    0.199767] virtio_rpmsg_bus virtio0: creating channel rpmsg_mrfl_thermal addr 0x25
[    0.199897] virtio_rpmsg_bus virtio0: creating channel rpmsg_mid_powerbtn addr 0x10
[    0.200022] virtio_rpmsg_bus virtio0: creating channel rpmsg_pmic_ccsm addr 0x19
[    0.200158] virtio_rpmsg_bus virtio0: creating channel rpmsg_msic_gpio addr 0x5
[    0.200285] virtio_rpmsg_bus virtio0: creating channel rpmsg_ipc_command addr 0xa0
[    0.200411] virtio_rpmsg_bus virtio0: creating channel rpmsg_ipc_simple_command addr 0xa1
[    0.200538] virtio_rpmsg_bus virtio0: creating channel rpmsg_ipc_raw_command addr 0xa2
[    0.200675] virtio_rpmsg_bus virtio0: creating channel rpmsg_pmic addr 0xff
[    0.200803] virtio_rpmsg_bus virtio0: creating channel rpmsg_mip addr 0xec
[    0.200932] virtio_rpmsg_bus virtio0: creating channel rpmsg_fw_update addr 0x13
[    0.201071] virtio_rpmsg_bus virtio0: creating channel rpmsg_ipc_util addr 0x12
[    0.201202] virtio_rpmsg_bus virtio0: creating channel rpmsg_flis addr 0xf5
[    0.201331] virtio_rpmsg_bus virtio0: creating channel rpmsg_watchdog addr 0xf8
[    0.201469] virtio_rpmsg_bus virtio0: creating channel rpmsg_umip addr 0x14
[    0.201601] virtio_rpmsg_bus virtio0: creating channel rpmsg_osip addr 0x15
[    0.201742] virtio_rpmsg_bus virtio0: creating channel rpmsg_vrtc addr 0xfa
[    0.201874] virtio_rpmsg_bus virtio0: creating channel rpmsg_fw_logging addr 0x27
[    0.202016] virtio_rpmsg_bus virtio0: creating channel rpmsg_kpd_led addr 0x23
[    0.202150] virtio_rpmsg_bus virtio0: creating channel rpmsg_modem_nvram addr 0xa2
[    0.202285] virtio_rpmsg_bus virtio0: creating channel rpmsg_mid_pwm addr 0x22
[    0.202427] virtio_rpmsg_bus virtio0: rpmsg host is online
[    0.202521] intel_mid_rpmsg rpmsg5: Probed rpmsg_ipc device rpmsg_ipc_command
[    0.202542] intel_mid_rpmsg rpmsg5: Allocating rpmsg_instance
[    0.202585] intel_mid_rpmsg rpmsg6: Probed rpmsg_ipc device rpmsg_ipc_simple_command
[    0.202605] intel_mid_rpmsg rpmsg6: Allocating rpmsg_instance
[    0.202644] intel_mid_rpmsg rpmsg7: Probed rpmsg_ipc device rpmsg_ipc_raw_command
[    0.202664] intel_mid_rpmsg rpmsg7: Allocating rpmsg_instance
[    0.203098] Advanced Linux Sound Architecture Driver Initialized.
[    0.203116] Intel MID platform detected, using MID PCI ops
[    0.203128] PCI: Probing PCI hardware
[    0.203143] PCI: root bus 00: using default resources
[    0.203156] PCI: Probing PCI hardware (bus 00)
[    0.203348] PCI host bridge to bus 0000:00
[    0.203377] pci_bus 0000:00: root bus resource [io  0x0000-0xffff]
[    0.203399] pci_bus 0000:00: root bus resource [mem 0x00000000-0xfffffffff]
[    0.203418] pci_bus 0000:00: No busn resource found for root bus, will use [bus 00-ff]
[    0.203475] pci 0000:00:00.0: [8086:1170] type 00 class 0x060000
[    0.203805] pci 0000:00:01.0: [8086:1190] type 00 class 0x080501
[    0.203872] pci 0000:00:01.0: reg 10: [mem 0xff3fc000-0xff3fc0ff]
[    0.204061] pci 0000:00:01.0: PME# supported from D0 D3hot
[    0.204335] pci 0000:00:01.2: [8086:1190] type 00 class 0x080501
[    0.204398] pci 0000:00:01.2: reg 10: [mem 0xff3fa000-0xff3fa0ff]
[    0.204584] pci 0000:00:01.2: PME# supported from D0 D3hot
[    0.204843] pci 0000:00:01.3: [8086:1190] type 00 class 0x080501
[    0.204905] pci 0000:00:01.3: reg 10: [mem 0xff3fb000-0xff3fb0ff]
[    0.205091] pci 0000:00:01.3: PME# supported from D0 D3hot
[    0.205375] pci 0000:00:02.0: [8086:1182] type 00 class 0x038000
[    0.205441] pci 0000:00:02.0: reg 10: [mem 0xc0000000-0xc1ffffff]
[    0.205499] pci 0000:00:02.0: reg 18: [mem 0x80000000-0x8fffffff]
[    0.205556] pci 0000:00:02.0: reg 20: [io  0x7ff8-0x7fff]
[    0.205905] pci 0000:00:04.0: [8086:1191] type 00 class 0x070002
[    0.205965] pci 0000:00:04.0: reg 10: [mem 0xff010000-0xff01007f]
[    0.206151] pci 0000:00:04.0: PME# supported from D0 D3hot
[    0.206418] pci 0000:00:04.1: [8086:1191] type 00 class 0x070002
[    0.206480] pci 0000:00:04.1: reg 10: [mem 0xff010080-0xff0100ff]
[    0.206666] pci 0000:00:04.1: PME# supported from D0 D3hot
[    0.206934] pci 0000:00:04.2: [8086:1191] type 00 class 0x070002
[    0.206996] pci 0000:00:04.2: reg 10: [mem 0xff010100-0xff01017f]
[    0.207183] pci 0000:00:04.2: PME# supported from D0 D3hot
[    0.207443] pci 0000:00:04.3: [8086:1191] type 00 class 0x070002
[    0.207504] pci 0000:00:04.3: reg 10: [mem 0xff010180-0xff0101ff]
[    0.207691] pci 0000:00:04.3: PME# supported from D0 D3hot
[    0.207970] pci 0000:00:05.0: [8086:1192] type 00 class 0x070002
[    0.208032] pci 0000:00:05.0: reg 10: [mem 0xff010400-0xff0107ff]
[    0.208218] pci 0000:00:05.0: PME# supported from D0 D3hot
[    0.208488] pci 0000:00:06.0: [8086:1193] type 00 class 0x088000
[    0.208550] pci 0000:00:06.0: reg 10: [mem 0xff2a0000-0xff2a0fff]
[    0.208736] pci 0000:00:06.0: PME# supported from D0 D3hot
[    0.209037] pci 0000:00:06.1: [8086:1193] type 00 class 0x088000
[    0.209100] pci 0000:00:06.1: reg 10: [mem 0xff2a1000-0xff2a1fff]
[    0.209287] pci 0000:00:06.1: PME# supported from D0 D3hot
[    0.209611] pci 0000:00:07.0: [8086:1194] type 00 class 0x088000
[    0.209674] pci 0000:00:07.0: reg 10: [mem 0xff188000-0xff188fff]
[    0.209860] pci 0000:00:07.0: PME# supported from D0 D3hot
[    0.210126] pci 0000:00:07.1: [8086:1194] type 00 class 0x088000
[    0.210187] pci 0000:00:07.1: reg 10: [mem 0xff189000-0xff189fff]
[    0.210374] pci 0000:00:07.1: PME# supported from D0 D3hot
[    0.210638] pci 0000:00:07.2: [8086:1194] type 00 class 0x088000
[    0.210699] pci 0000:00:07.2: reg 10: [mem 0xff18a000-0xff18afff]
[    0.210885] pci 0000:00:07.2: PME# supported from D0 D3hot
[    0.211163] pci 0000:00:08.0: [8086:1195] type 00 class 0x078000
[    0.211225] pci 0000:00:08.0: reg 10: [mem 0xff18b000-0xff18bfff]
[    0.211411] pci 0000:00:08.0: PME# supported from D0 D3hot
[    0.211667] pci 0000:00:08.1: [8086:1195] type 00 class 0x078000
[    0.211728] pci 0000:00:08.1: reg 10: [mem 0xff18c000-0xff18cfff]
[    0.211913] pci 0000:00:08.1: PME# supported from D0 D3hot
[    0.212178] pci 0000:00:08.2: [8086:1195] type 00 class 0x078000
[    0.212240] pci 0000:00:08.2: reg 10: [mem 0xff18d000-0xff18dfff]
[    0.212427] pci 0000:00:08.2: PME# supported from D0 D3hot
[    0.212694] pci 0000:00:08.3: [8086:1195] type 00 class 0x078000
[    0.212756] pci 0000:00:08.3: reg 10: [mem 0xff18e000-0xff18efff]
[    0.212943] pci 0000:00:08.3: PME# supported from D0 D3hot
[    0.213213] pci 0000:00:09.0: [8086:1196] type 00 class 0x078000
[    0.213274] pci 0000:00:09.0: reg 10: [mem 0xff18f000-0xff18ffff]
[    0.213460] pci 0000:00:09.0: PME# supported from D0 D3hot
[    0.213728] pci 0000:00:09.1: [8086:1196] type 00 class 0x078000
[    0.213789] pci 0000:00:09.1: reg 10: [mem 0xff190000-0xff190fff]
[    0.213976] pci 0000:00:09.1: PME# supported from D0 D3hot
[    0.214233] pci 0000:00:09.2: [8086:1196] type 00 class 0x078000
[    0.214294] pci 0000:00:09.2: reg 10: [mem 0xff191000-0xff191fff]
[    0.214481] pci 0000:00:09.2: PME# supported from D0 D3hot
[    0.214764] pci 0000:00:0a.0: [8086:1197] type 00 class 0x078000
[    0.214826] pci 0000:00:0a.0: reg 10: [mem 0xff3f8000-0xff3f8fff]
[    0.215012] pci 0000:00:0a.0: PME# supported from D0 D3hot
[    0.215282] pci 0000:00:0b.0: [8086:1198] type 00 class 0x108000
[    0.215344] pci 0000:00:0b.0: reg 10: [mem 0xf9038000-0xf903ffff]
[    0.215530] pci 0000:00:0b.0: PME# supported from D0 D3hot
[    0.215791] pci 0000:00:0c.0: [8086:1199] type 00 class 0x088000
[    0.215852] pci 0000:00:0c.0: reg 10: [mem 0xff008000-0xff008fff]
[    0.215892] pci 0000:00:0c.0: reg 14: [mem 0x000df570-0x000df57f]
[    0.216062] pci 0000:00:0c.0: PME# supported from D0 D3hot
[    0.216333] pci 0000:00:0d.0: [8086:119a] type 00 class 0x040100
[    0.216395] pci 0000:00:0d.0: reg 10: [mem 0x05e00000-0x05ffffff]
[    0.216435] pci 0000:00:0d.0: reg 14: [mem 0xff340000-0xff343fff]
[    0.216473] pci 0000:00:0d.0: reg 18: [mem 0xff344000-0xff344fff]
[    0.216510] pci 0000:00:0d.0: reg 1c: [mem 0xff2c0000-0xff2dffff]
[    0.216548] pci 0000:00:0d.0: reg 20: [mem 0xff300000-0xff33ffff]
[    0.216670] pci 0000:00:0d.0: PME# supported from D0 D3hot
[    0.216940] pci 0000:00:0e.0: [8086:119b] type 00 class 0x088000
[    0.217001] pci 0000:00:0e.0: reg 10: [mem 0xff298000-0xff29bfff]
[    0.217040] pci 0000:00:0e.0: reg 14: [mem 0xff2a2000-0xff2a2fff]
[    0.217210] pci 0000:00:0e.0: PME# supported from D0 D3hot
[    0.217479] pci 0000:00:11.0: [8086:119e] type 00 class 0x0c0320
[    0.217584] pci 0000:00:11.0: reg 10: [mem 0xf9100000-0xf911ffff]
[    0.217773] pci 0000:00:11.0: PME# supported from D0 D3hot
[    0.218046] pci 0000:00:12.0: [8086:119f] type 00 class 0x118000
[    0.218109] pci 0000:00:12.0: reg 10: [mem 0xf9009000-0xf9009fff]
[    0.218148] pci 0000:00:12.0: reg 14: [mem 0xf90a0000-0xf90affff]
[    0.218186] pci 0000:00:12.0: reg 18: [mem 0xfa000000-0xfaffffff]
[    0.218340] pci 0000:00:12.0: PME# supported from D0 D3hot
[    0.218621] pci 0000:00:13.0: [8086:11a0] type 00 class 0x0b4000
[    0.218682] pci 0000:00:13.0: reg 10: [mem 0xff009000-0xff009fff]
[    0.218869] pci 0000:00:13.0: PME# supported from D0 D3hot
[    0.219171] pci 0000:00:14.0: [8086:11a1] type 00 class 0x0b4000
[    0.219234] pci 0000:00:14.0: reg 10: [mem 0xff00b000-0xff00bfff]
[    0.219421] pci 0000:00:14.0: PME# supported from D0 D3hot
[    0.219697] pci 0000:00:15.0: [8086:11a2] type 00 class 0x088000
[    0.219759] pci 0000:00:15.0: reg 10: [mem 0xff192000-0xff192fff]
[    0.219945] pci 0000:00:15.0: PME# supported from D0 D3hot
[    0.220208] pci 0000:00:16.0: [8086:11a3] type 00 class 0x0b4000
[    0.220270] pci 0000:00:16.0: reg 10: [mem 0xff0d9000-0xff0d90ff]
[    0.220456] pci 0000:00:16.0: PME# supported from D0 D3hot
[    0.220729] pci 0000:00:16.1: [8086:11a4] type 00 class 0x0b4000
[    0.220791] pci 0000:00:16.1: reg 10: [mem 0x04819000-0x04898fff]
[    0.220831] pci 0000:00:16.1: reg 14: [mem 0x04919000-0x04920fff]
[    0.221001] pci 0000:00:16.1: PME# supported from D0 D3hot
[    0.221298] pci 0000:00:17.0: [8086:11a5] type 00 class 0x088000
[    0.221358] pci 0000:00:17.0: reg 10: [mem 0xff013000-0xff013fff]
[    0.221545] pci 0000:00:17.0: PME# supported from D0 D3hot
[    0.221842] pci 0000:00:18.0: [8086:11a6] type 00 class 0x038000
[    0.222063] pci 0000:00:18.0: PME# supported from D0 D3hot
[    0.222368] pci_bus 0000:00: busn_res: [bus 00-ff] end is updated to 00
[    0.222484] PCI: pci_cache_line_size set to 64 bytes
[    0.222738] e820: reserve RAM buffer [mem 0x00098000-0x0009ffff]
[    0.222757] e820: reserve RAM buffer [mem 0x3f500000-0x3fffffff]
[    0.223359] Bluetooth: Core ver 2.16
[    0.223430] NET: Registered protocol family 31
[    0.223445] Bluetooth: HCI device and connection manager initialized
[    0.223470] Bluetooth: HCI socket layer initialized
[    0.223491] Bluetooth: L2CAP socket layer initialized
[    0.223542] Bluetooth: SCO socket layer initialized
[    0.224026] cfg80211: Calling CRDA to update world regulatory domain
[    0.224070] NetLabel: Initializing
[    0.224088] NetLabel:  domain hash size = 128
[    0.224099] NetLabel:  protocols = UNLABELED CIPSOv4
[    0.224188] NetLabel:  unlabeled traffic allowed by default
[    0.225315] intel_scu_flis platform device created
[    0.225388] hsu core clock 38 M
[    0.225546] intel_pmu_driver 0000:00:14.0: PMU DRIVER Probe called
[    0.226687] intel_pmu_driver 0000:00:14.0: after pmu initialization
[    0.226837] Switching to clocksource refined-jiffies
[    0.403610] intel_scu_flis rpmsg12: Probed flis rpmsg device
[    0.403637] intel_scu_flis rpmsg12: Allocating rpmsg_instance
[    0.403767] intel_scu_flis intel_scu_flis: scu flis probed
[    0.417419] pci_bus 0000:00: resource 4 [io  0x0000-0xffff]
[    0.417446] pci_bus 0000:00: resource 5 [mem 0x00000000-0xfffffffff]
[    0.417623] NET: Registered protocol family 2
[    0.418895] TCP established hash table entries: 8192 (order: 4, 65536 bytes)
[    0.419073] TCP bind hash table entries: 8192 (order: 4, 65536 bytes)
[    0.419239] TCP: Hash tables configured (established 8192 bind 8192)
[    0.419322] TCP: reno registered
[    0.419346] UDP hash table entries: 512 (order: 2, 16384 bytes)
[    0.419393] UDP-Lite hash table entries: 512 (order: 2, 16384 bytes)
[    0.419702] NET: Registered protocol family 1
[    0.420095] RPC: Registered named UNIX socket transport module.
[    0.420112] RPC: Registered udp transport module.
[    0.420125] RPC: Registered tcp transport module.
[    0.420136] RPC: Registered tcp NFSv4.1 backchannel transport module.
[    0.422566] PCI: CLS 0 bytes, default 64
[    0.422639] intel_scu_pmic rpmsg8: Probed pmic rpmsg device
[    0.422659] intel_scu_pmic rpmsg8: Allocating rpmsg_instance
[    0.423184] intel_scu_watchdog_evo rpmsg13: Probed watchdog rpmsg device
[    0.423206] intel_scu_watchdog_evo rpmsg13: Allocating rpmsg_instance
[    0.423772] intel_scu_ipcutil rpmsg11: Probed ipcutil rpmsg device
[    0.423794] intel_scu_ipcutil rpmsg11: Allocating rpmsg_instance
[    0.423910] (oshob) base addr = 0xfffff000
[    0.423924] (oshob) identified platform = INTEL_MID_CPU_CHIP_TANGIER
[    0.423941] (oshob) oshob version = 1.4
[    0.423989] (latest extend oshob) osnib ptr = 0xfffff800
[    0.424003] Using latest extended oshob structure size = 1024 bytes
[    0.424016] OSNIB Intel size = 32 bytes OEMNIB size = 96 bytes
[    0.424029] (extend oshob) SCU buffer size is 16 bytes
[    0.424093] [BOOT] RESETSRC0=0x00 RESETSRC1=0x00 (PMIT interrupt tree)
[    0.424164] [BOOT] SCU_TR[0]=0x00020011
[    0.424178] [BOOT] SCU_TR[1]=0x00000220
[    0.424191] [BOOT] SCU_TR[2]=0x00000000
[    0.424203] [BOOT] SCU_TR[3]=0x00000000
[    0.424214] [BOOT] IA_TR=0x00000000 (oshob)
[    0.424545] [BOOT] RR=[fastboot] WD=0x00 ALARM=0x00 (osnib)
[    0.424560] [BOOT] WAKESRC=[real reset] (osnib)
[    0.424574] [BOOT] RESETSRC0=0x00 RESETSRC1=0x02 (osnib)
[    0.424624] OEMNIB interface registered to debugfs
[    0.424926] iio_basincove_gpadc rpmsg0: Probed bcove_gpadc rpmsg device
[    0.425483] bcove_adc bcove_adc: bcove adc probed
[    0.426425] platform rtc_cmos: registered platform RTC device (no PNP device found)
[    0.429814] vprog1: 1500 <--> 2800 mV at 2800 mV normal 
[    0.430401] vprog2: 1500 <--> 2850 mV at 2850 mV normal 
[    0.430970] vprog3: 1050 <--> 2800 mV at 1050 mV normal 
[    0.574737] bounce pool size: 64 pages
[    0.586808] NFS: Registering the id_resolver key type
[    0.586870] Key type id_resolver registered
[    0.586886] Key type id_legacy registered
[    0.586915] Installing knfsd (copyright (C) 1996 okir@monad.swb.de).
[    0.587511] fuse init (API version 7.22)
[    0.588131] msgmni has been set to 1670
[    0.590769] Key type asymmetric registered
[    0.590790] Asymmetric key parser 'x509' registered
[    0.591048] Block layer SCSI generic (bsg) driver version 0.4 loaded (major 249)
[    0.591246] io scheduler noop registered
[    0.591448] io scheduler cfq registered (default)
[    0.591463] list_sort_test: start testing list_sort()
[    0.594072] intel_idle: MWAIT substates: 0x33000020
[    0.594091] intel_idle: v0.4 model 0x4A
[    0.594105] intel_idle: lapic_timer_reliable_states 0xffffffff
[    0.594346] intel_mid_dma 0000:00:0e.0: setting latency timer to 64
[    0.594879] intel_mid_dma 0000:00:15.0: setting latency timer to 64
[    0.596188] HSU DMA 0000:00:05.0: FUNC: 0 driver: 5 addr:ff010400 len:400
[    0.596404] HSU serial 0000:00:04.0: FUNC: 0 driver: 0 addr:ff010000 len:80
[    0.596452] HSU serial 0000:00:04.1: FUNC: 1 driver: 0 addr:ff010080 len:80
[    0.596520] Found a Intel HSU
[    0.597161] 0000:00:04.1: ttyMFD0 at MMIO 0xff010080 (irq = 28) is a hsu_bt_port_p
[    0.597716] HSU serial 0000:00:04.2: FUNC: 2 driver: 0 addr:ff010100 len:80
[    0.597790] Found a Intel HSU
[    0.598406] 0000:00:04.2: ttyMFD1 at MMIO 0xff010100 (irq = 29) is a hsu_uart1_port_p
[    0.598837] HSU serial 0000:00:04.3: FUNC: 3 driver: 0 addr:ff010180 len:80
[    0.598913] Found a Intel HSU
[    0.599433] 0000:00:04.3: ttyMFD2 at MMIO 0xff010180 (irq = 54) is a hsu_uart2_port_p
[    0.619989] console [ttyMFD2] enabled
[    0.620945] Non-volatile memory driver v1.3
[    0.621536] Linux agpgart interface v0.103
[    0.622389] tpm_tis tpm_tis: 1.2 TPM (device-id 0xFFFF, rev-id 255)
[    0.622419] tpm_tis tpm_tis: Unable to request irq: 255 for probe
[    0.622458] tpm_tis tpm_tis: tpm_transmit: tpm_send: error -5
[    0.622537] tpm_tis tpm_tis: A TPM error (-5) occurred attempting to determine the timeouts
[    0.622641] tpm_tis tpm_tis: tpm_transmit: tpm_send: error -5
[    0.622703] tpm_tis tpm_tis: Could not get TPM timeouts and durations
[    0.670049] [drm] Initialized drm 1.1.0 20060810
[    0.681084] brd: module loaded
[    0.686945] loop: module loaded
[    0.687984] emmc_ipanic: init success
[    0.688459] tun: Universal TUN/TAP device driver, 1.6
[    0.688476] tun: (C) 1999-2004 Max Krasnyansky <maxk@qualcomm.com>
[    0.688986] dwc3_otg 0000:00:11.0: setting latency timer to 64
[    0.690736] ehci_hcd: USB 2.0 'Enhanced' Host Controller (EHCI) Driver
[    0.690993] usbcore: registered new interface driver cdc_acm
[    0.691010] cdc_acm: USB Abstract Control Model driver for USB modems and ISDN adapters
[    0.691091] usbcore: registered new interface driver usb-storage
[    0.691244] usbcore: registered new interface driver usbserial
[    0.691305] usbcore: registered new interface driver usbserial_generic
[    0.691359] usbserial: USB Serial support registered for generic
[    0.692160] rtc_cmos rtc_cmos: rtc core: registered rtc_cmos as rtc0
[    0.692304] rtc_cmos rtc_cmos: alarms up to one day, 114 bytes nvram
[    0.692356] i2c /dev entries driver
[    0.840520] coretemp: Enabled Aux0/Aux1 interrupts for coretemp
[    0.840611] coretemp: Enabled Aux0/Aux1 interrupts for coretemp
[    0.940216] MCU detected and ready to used!
[    0.940329] bcove_thrm rpmsg1: Probed mrfl_thermal rpmsg device
[    0.943974] thermal thermal_zone0: failed to read out thermal zone 0
[    0.944426] thermal thermal_zone1: failed to read out thermal zone 1
[    0.944882] thermal thermal_zone2: failed to read out thermal zone 2
[    0.946888] Bluetooth: HCI UART driver ver 2.2
[    0.946908] Bluetooth: HCI H4 protocol initialized
[    0.947253] cpuidle: using governor ladder
[    0.947715] cpuidle: using governor menu
[    0.947773] sdhci: Secure Digital Host Controller Interface driver
[    0.947786] sdhci: Copyright(c) Pierre Ossman
[    0.947850] sdhci-pci 0000:00:01.0: SDHCI controller found [8086:1190] (rev 1)
[    0.947928] flis_addr mapped addr: f809c900
[    0.948034] sdhci-pci 0000:00:01.0: rte_addr mapped addr: f80aa000
[    0.948092] sdhci-pci 0000:00:01.0: setting latency timer to 64
[    0.948118] mmc0: no vqmmc regulator found
[    1.042563] mmc0: BKOPS_EN bit is not set
[    1.351389] mmc0: new HS200 MMC card at address 0001
[    1.352091] mmcblk0: mmc0:0001 H4G1d 3.64 GiB 
[    1.352445] mmcblk0boot0: mmc0:0001 H4G1d partition 1 4.00 MiB
[    1.352787] mmcblk0boot1: mmc0:0001 H4G1d partition 2 4.00 MiB
[    1.353142] mmcblk0rpmb: mmc0:0001 H4G1d partition 3 4.00 MiB
[    1.358569]  mmcblk0: p1 p2 p3 p4 p5 p6 p7 p8 p9 p10
[    1.365806]  mmcblk0boot1: unknown partition table
[    1.369274]  mmcblk0boot0: unknown partition table
[    1.369609] mmc0: SDHCI controller on PCI [0000:00:01.0] using ADMA
[    1.384274] emmc_ipanic: panic partition found, label:panic, device:mmcblk0p6
[    1.420568] Switching to clocksource tsc
[    1.476695] emmc_ipanic: emmc_panic_notify_add: Data available in panic partition
[    1.476742] emmc_ipanic: emmc_panic_notify_add: proc entry created: emmc_ipanic_header
[    1.476838] emmc_ipanic: emmc_panic_notify_add: log file 0(1024, 40493)
[    1.476869] emmc_ipanic: emmc_panic_notify_add: proc entry created: emmc_ipanic_console
[    1.476886] emmc_ipanic: emmc_panic_notify_add: log file 1(4286578688, 0)
[    1.476899] emmc_ipanic: emmc_panic_notify_add: empty log file 1
[    1.476913] emmc_ipanic: emmc_panic_notify_add: log file 2(4286578688, 0)
[    1.476926] emmc_ipanic: emmc_panic_notify_add: empty log file 2
[    1.477008] sdhci-pci 0000:00:01.2: SDHCI controller found [8086:1190] (rev 1)
[    1.501101] sdhci-pci 0000:00:01.2: setting latency timer to 64
[    1.501137] mmc1: no vqmmc regulator found
[    1.501496] mmc1: SDHCI controller on PCI [0000:00:01.2] using ADMA
[    1.501658] sdhci-pci 0000:00:01.3: SDHCI controller found [8086:1190] (rev 1)
[    1.501764] vwlan gpio 96
[    1.502054] vwlan: 1800 mV 
[    1.502265] sdhci-pci 0000:00:01.3: setting latency timer to 64
[    1.502301] mmc2: no vqmmc regulator found
[    1.502646] mmc2: SDHCI controller on PCI [0000:00:01.3] using ADMA
[    1.511457] hidraw: raw HID events driver (C) Jiri Kosina
[    1.512004] usbcore: registered new interface driver usbhid
[    1.512022] usbhid: USB HID core driver
[    1.512107] intel_scu_fw_update rpmsg10: Probed fw_update rpmsg device
[    1.512128] intel_scu_fw_update rpmsg10: Allocating rpmsg_instance
[    1.516837] usbcore: registered new interface driver snd-usb-audio
[    1.517386] snd_intel_sst: INFO: ******** SST DRIVER loading.. Ver: 3.0.8
[    1.518059] snd_intel_sst: Got drv data max stream 25
[    1.519776] snd_intel_sst: intel_sst_probe successfully done!
[    1.519981] oprofile: using NMI interrupt.
[    1.520104] Netfilter messages via NETLINK v0.30.
[    1.520196] nf_conntrack version 0.5.0 (15360 buckets, 61440 max)
[    1.521200] TCP: cubic registered
[    1.521216] Initializing XFRM netlink socket
[    1.521917] NET: Registered protocol family 10
[    1.523025] sit: IPv6 over IPv4 tunneling driver
[    1.523781] NET: Registered protocol family 17
[    1.523830] NET: Registered protocol family 15
[    1.523931] Bridge firewalling registered
[    1.524037] snd_intel_sst: runtime_idle called
[    1.524056] snd_intel_sst: runtime_suspend called
[    1.524282] Bluetooth: RFCOMM TTY layer initialized
[    1.524338] Bluetooth: RFCOMM socket layer initialized
[    1.524355] Bluetooth: RFCOMM ver 1.11
[    1.524371] Bluetooth: BNEP (Ethernet Emulation) ver 1.3
[    1.524384] Bluetooth: BNEP filters: protocol multicast
[    1.524409] Bluetooth: BNEP socket layer initialized
[    1.524423] Bluetooth: HIDP (Human Interface Emulation) ver 1.2
[    1.524445] Bluetooth: HIDP socket layer initialized
[    1.524600] l2tp_core: L2TP core driver, V2.0
[    1.524672] Key type dns_resolver registered
[    1.528640] Using IPI No-Shortcut mode
[    1.528692] info[ 0]: name = power_btn, gpio = -1
[    1.528708] info[ 1]: name = SW1UI4, gpio = 61
[    1.529942] registered taskstats version 1
[    1.529961] IMA: No TPM chip found, activating TPM-bypass!
[    1.532782] vwlan: incomplete constraints, leaving on
[    1.534494] regulator-dummy: incomplete constraints, leaving on
[    1.536208] intel_mid_ssp_spi_unified 0000:00:07.0: found PCI SSP controller (ID: 8086h:1194h cfg: )
[    1.539373] intel_mid_ssp_spi_unified 0000:00:07.0: register with SPI framework (bus spi3)
[    1.539500] intel_mid_ssp_spi_unified 0000:00:07.0: master is unqueued, this is deprecated
[    1.539528] intel_mid_ssp_spi_unified 0000:00:07.0: Unbalanced pm_runtime_enable!
[    1.540772] intel_mid_ssp_spi_unified 0000:00:07.1: found PCI SSP controller (ID: 8086h:1194h cfg: )
[    1.542646] intel_mid_ssp_spi_unified 0000:00:07.1: register with SPI framework (bus spi5)
[    1.542782] intel_mid_ssp_spi_unified 0000:00:07.1: master is unqueued, this is deprecated
[    1.546302] intel_mid_ssp_spi_unified 0000:00:07.1: Unbalanced pm_runtime_enable!
[    1.550829] intel_mid_ssp_spi_unified 0000:00:07.2: found PCI SSP controller (ID: 8086h:1194h cfg: )
[    1.551697] intel_mid_ssp_spi_unified 0000:00:07.2: register with SPI framework (bus spi6)
[    1.551829] intel_mid_ssp_spi_unified 0000:00:07.2: master is unqueued, this is deprecated
[    1.551857] intel_mid_ssp_spi_unified 0000:00:07.2: Unbalanced pm_runtime_enable!
[    1.561140] console [netcon0] enabled
[    1.561159] netconsole: network logging started
[    1.561692] input: gpio-keys as /devices/platform/gpio-keys/input/input0
[    1.562355] rtc_cmos rtc_cmos: setting system clock to 2000-01-01 00:00:09 UTC (946684809)
[    1.562426] pmic_ccsm rpmsg3: Probed pmic_ccsm rpmsg device
[    1.562794] pmic_ccsm pmic_ccsm: PMIC-ID: c9
[    1.562816] pmic_ccsm pmic_ccsm: Error reading battery profile from battid frmwrk
[    1.572425] pmic_ccsm pmic_ccsm: Battery Over heat exception
[    1.572502] pmic_ccsm pmic_ccsm: Battery0 temperature inside boundary
[    1.572564] pmic_ccsm pmic_ccsm: USB VBUS Detected. Notifying OTG driver
[    1.572710] pmic_ccsm pmic_ccsm: Battery Zone changed. Current zone is 5
[    1.587621] APIC ID: 0
[    1.587638] APIC ID: 2
[    1.587676] Num p-states 2
[    1.587693] State [0]: core_frequency[500] transition_latency[100] control[0x529]
[    1.587708] State [1]: core_frequency[500] transition_latency[100] control[0x529]
[    1.587835] Num p-states 2
[    1.587852] State [0]: core_frequency[500] transition_latency[100] control[0x529]
[    1.587867] State [1]: core_frequency[500] transition_latency[100] control[0x529]
[    1.588188] msic_power_btn rpmsg2: Probed mid_pb rpmsg device
[    1.588244] msic_power_btn mid_powerbtn: Probed mid powerbutton devivce
[    1.588527] input: mid_powerbtn as /devices/platform/mid_powerbtn/input/input1
[    1.591232] ALSA device list:
[    1.591252]   #0: Loopback 1
[    1.662925] EXT4-fs (mmcblk0p8): mounted filesystem with ordered data mode. Opts: (null)
[    1.663007] VFS: Mounted root (ext4 filesystem) readonly on device 179:8.
[    1.665312] devtmpfs: mounted
[    1.665638] Freeing unused kernel memory: 512k freed
[    1.666271] Write protecting the kernel text: 6932k
[    1.666841] Write protecting the kernel read-only data: 2820k
[    1.666854] NX-protecting the kernel data: 5356k
[    1.806422] systemd[1]: Successfully loaded Smack policies.
[    1.807394] systemd[1]: System time before build time, advancing clock.
[    1.825630] ip_tables: (C) 2000-2006 Netfilter Core Team
[    1.839606] systemd[1]: Relabelled /dev and /run in 8.739ms.
[    1.904837] systemd[1]: systemd 229 running in system mode. (+PAM -AUDIT -SELINUX +IMA -APPARMOR +S)
[    1.906028] systemd[1]: Detected architecture x86.
[    1.992626] systemd[1]: Set hostname to <edison>.
[    1.994485] systemd[1]: Initializing machine ID from random generator.
[    1.994792] systemd[1]: Installed transient /etc/machine-id file.
[    1.995936] systemd[1]: Hardware watchdog 'Intel_SCU IOH Watchdog', version 0
[    1.995995] systemd[1]: Set hardware watchdog to 1min 30s.
[    2.039103] mmc2: queuing unknown CIS tuple 0x91 (3 bytes)
[    2.039143] mmc2: new ultra high speed DDR50 SDIO card at address 0001
[    2.596640] systemd[1]: Created slice User and Session Slice.
[    2.641320] systemd[1]: Listening on /dev/initctl Compatibility Named Pipe.
[    2.691681] systemd[1]: Created slice System Slice.
[    2.731711] systemd[1]: Created slice system-getty.slice.
[    2.771654] systemd[1]: Created slice system-wpa_supplicant.slice.
[    2.810802] systemd[1]: Reached target Slices.
[    2.851629] systemd[1]: Created slice system-serial\x2dgetty.slice.
[    2.891211] systemd[1]: Started Dispatch Password Requests to Console Directory Watch.
[    2.931183] systemd[1]: Listening on Journal Socket (/dev/log).
[    2.971140] systemd[1]: Started Forward Password Requests to Wall Directory Watch.
[    3.011088] systemd[1]: Listening on Journal Socket.
[    3.053824] systemd[1]: Starting File System Check on Root Device...
[    3.107553] systemd[1]: Starting ip6tables firewall...
[    3.137767] systemd[1]: Mounting Temporary Directory...
[    3.153197] ip6_tables: (C) 2000-2006 Netfilter Core Team
[    3.166045] systemd[1]: Starting iptables firewall...
[    3.232482] systemd[1]: Starting Create list of required static device nodes for the current kernel.
[    3.267194] systemd[1]: Starting Setup Virtual Console...
[    3.334149] systemd[1]: Mounting Debug File System...
[    3.436668] systemd[1]: Starting Load Kernel Modules...
[    3.450743] systemd[1]: Listening on udev Kernel Socket.
[    3.465937] dhd_module_init in
[    3.465968] found wifi platform device wlan
[    3.466061] Power-up adapter 'DHD generic adapter'
[    3.466774] systemd[1]: Listening on Network Service Netlink Socket.
[    3.520674] systemd[1]: Reached target Swap.
[    3.574189] systemd[1]: Starting Journal Service...
[    3.610757] systemd[1]: Reached target Paths.
[    3.659370] systemd[1]: Mounting POSIX Message Queue File System...
[    3.690777] systemd[1]: Reached target Remote File Systems.
[    3.731111] systemd[1]: Listening on udev Control Socket.
[    3.783726] systemd[1]: Mounted Debug File System.
[    3.820940] systemd[1]: Mounted POSIX Message Queue File System.
[    3.863413] systemd[1]: Mounted Temporary Directory.
[    3.872796] wifi_platform_set_power = 1
[    3.912569] systemd[1]: Started File System Check on Root Device.
[    3.952471] systemd[1]: Started ip6tables firewall.
[    3.993182] systemd[1]: Started iptables firewall.
[    4.032378] systemd[1]: Started Create list of required static device nodes for the current kernel.
[    4.072394] systemd[1]: Started Setup Virtual Console.
[    4.080380] wifi_platform_bus_enumerate device present 1
[    4.102864] systemd[1]: Started Journal Service.
[    4.106363] bcmsdh_sdmmc: bcmsdh_sdmmc_probe Enter
[    4.106601] bcmsdh_sdmmc: bcmsdh_sdmmc_probe Enter
[    4.106621] bus num (host idx)=2, slot num (rca)=1
[    4.106635] found adapter info 'DHD generic adapter'
[    4.116968] F1 signature OK, socitype:0x1 chip:0xa94c rev:0x2 pkg:0x0
[    4.118434] DHD: dongle ram size is set to 524288(orig 524288) at 0x0
[    4.120136] wifi_platform_get_mac_addr
[    4.120209] wifi_get_mac_addr_intel: unable to open /config/wifi/mac.txt
[    4.121041] wl_create_event_handler(): thread:wl_event_handler:8d started
[    4.121298] CFG80211-ERROR) wl_event_handler : tsk Enter, tsk = 0xf5501440
[    4.121381] dhd_attach(): thread:dhd_watchdog_thread:8e started
[    4.121520] dhd_attach(): thread:dhd_dpc:8f started
[    4.121547] dhd_deferred_work_init: work queue initialized 
[    4.123080] Dongle Host Driver, version 1.141.59 (r)
               Compiled in /var/lib/jenkins/ostro-worker-20-slot-1-jekA7/ostro-os/build/tmp-glibc/work3
[    4.123998] Register interface [wlan0]  MAC: 00:00:00:00:00:00

[    4.124025] dhd_prot_ioctl : bus is down. we have nothing to do
[    4.124629] bcmsdh_sdmmc: bcmsdh_sdmmc_probe Enter
[    4.124725] wifi_platform_set_power = 0
[    4.125805] wifi_platform_bus_enumerate device present 0
[    4.192618] g_multi gadget: using random host ethernet address
[    4.193518] usb0: MAC 02:00:86:58:c2:af
[    4.193540] usb0: HOST MAC d6:5f:95:62:24:3a
[    4.217156] g_multi gadget: Mass Storage Function, version: 2009/09/11
[    4.217182] g_multi gadget: Number of LUNs=1
[    4.217208]  lun0: LUN: file: /dev/mmcblk0p9
[    4.217404] g_multi gadget: Multifunction Composite Gadget
[    4.217423] g_multi gadget: g_multi ready
[    4.611622] EXT4-fs (mmcblk0p8): re-mounted. Opts: discard,barrier=1,data=ordered,noauto_da_alloc
[    5.175442] systemd-journald[138]: Received request to flush runtime journal from PID 1
[    5.478785] g_multi gadget: high-speed config #2: Multifunction with CDC ECM
[    8.315520] EXT4-fs (mmcblk0p5): mounted filesystem without journal. Opts: (null)
[   10.518580] 
               Dongle Host Driver, version 1.141.59 (r)
               Compiled in /var/lib/jenkins/ostro-worker-20-slot-1-jekA7/ostro-os/build/tmp-glibc/work3
[   10.518614] wl_android_wifi_on in
[   10.518630] wifi_platform_set_power = 1
[   11.124537] F1 signature OK, socitype:0x1 chip:0xa94c rev:0x2 pkg:0x0
[   11.125937] DHD: dongle ram size is set to 524288(orig 524288) at 0x0
[   11.128039] dhdsdio_download_firmware: firmware path=/etc/firmware/fw_bcmdhd.bin, nvram path=/etc/fl
[   11.345281] sdioh_request_buffer: [1] doing memory copy buf=f5671000, len=18
[   11.412528] cgroup: systemd (1) created nested cgroup for controller "blkio" which has incomplete h.
[   11.424223] dhdsdio_write_vars: Download, Upload and compare of NVRAM succeeded.
[   11.585369] dhd_bus_init: enable 0x06, ready 0x06 (waited 0us)
[   11.602360] wifi_platform_get_mac_addr
[   11.602859] wifi_get_mac_addr_intel: unable to open /config/wifi/mac.txt
[   11.607709] Firmware up: op_mode=0x0015, MAC=78:4b:87:a5:3a:73
[   11.629753] Firmware version = wl0: Jan 30 2015 19:22:32 version 6.20.190.3 (r530911) FWID 01-5b07cc
[   11.630680] dhd_preinit_ioctls wl ampdu_hostreorder failed -23
[   11.720962] CFG80211-ERROR) wl_update_wiphybands : bw_cap failed, -23
[   11.996823] wl_android_wifi_off in
[   12.005895] wifi_platform_set_power = 0
[  262.476923] 
               Dongle Host Driver, version 1.141.59 (r)
               Compiled in /var/lib/jenkins/ostro-worker-20-slot-1-jekA7/ostro-os/build/tmp-glibc/work3
[  262.476957] wl_android_wifi_on in
[  262.476973] wifi_platform_set_power = 1
[  263.066158] F1 signature OK, socitype:0x1 chip:0xa94c rev:0x2 pkg:0x0
[  263.067717] DHD: dongle ram size is set to 524288(orig 524288) at 0x0
[  263.070035] dhdsdio_download_firmware: firmware path=/etc/firmware/fw_bcmdhd.bin, nvram path=/etc/fl
[  263.190903] sdioh_request_buffer: [1] doing memory copy buf=f5675000, len=18
[  263.194481] dhdsdio_write_vars: Download, Upload and compare of NVRAM succeeded.
[  263.352961] dhd_bus_init: enable 0x06, ready 0x06 (waited 0us)
[  263.356067] wifi_platform_get_mac_addr
[  263.356143] wifi_get_mac_addr_intel: unable to open /config/wifi/mac.txt
[  263.361423] Firmware up: op_mode=0x0015, MAC=78:4b:87:a5:3a:73
[  263.382681] Firmware version = wl0: Jan 30 2015 19:22:32 version 6.20.190.3 (r530911) FWID 01-5b07cc
[  263.383587] dhd_preinit_ioctls wl ampdu_hostreorder failed -23
[  263.478031] CFG80211-ERROR) wl_update_wiphybands : bw_cap failed, -23
[  296.186724] CFG80211-ERROR) wl_cfg80211_connect : Connectting withf8:01:13:a8:2b:40 channel (1) ssi)

[  296.258280] wl_bss_connect_done succeeded with f8:01:13:a8:2b:40
[  296.347450] wl_bss_connect_done succeeded with f8:01:13:a8:2b:40
[  297.443600] IPv6: wlan0: IPv6 duplicate address fdf8:113:a82b:3a00:7a4b:87ff:fea5:3a73 detected!
[  336.534850] CFG80211-ERROR) wl_scan_timeout : timer expired
[  336.535086] CFG80211-ERROR) wl_escan_handler : WLC_E_STATUS_TIMEOUT : scan_request[f5ab8200]
[  336.535114] CFG80211-ERROR) wl_escan_handler : reason[0xffffffff]
[  336.563305] CFG80211-ERROR) wl_escan_handler : escan is not ready ndev f587d800 drv_status 0x0 e_ty4
[  376.569322] CFG80211-ERROR) wl_scan_timeout : timer expired
[  376.569430] CFG80211-ERROR) wl_escan_handler : WLC_E_STATUS_TIMEOUT : scan_request[f5ab8e00]
[  376.569456] CFG80211-ERROR) wl_escan_handler : reason[0xffffffff]
[  376.577146] CFG80211-ERROR) wl_escan_handler : escan is not ready ndev f587d800 drv_status 0x0 e_ty4
[  487.587921] CFG80211-ERROR) wl_scan_timeout : timer expired
[  487.588015] CFG80211-ERROR) wl_escan_handler : WLC_E_STATUS_TIMEOUT : scan_request[f5821f00]
[  487.588041] CFG80211-ERROR) wl_escan_handler : reason[0xffffffff]
[  487.610582] CFG80211-ERROR) wl_escan_handler : escan is not ready ndev f587d800 drv_status 0x0 e_ty8
[  487.610619] CFG80211-ERROR) wl_escan_handler : escan is not ready ndev f587d800 drv_status 0x0 e_ty4
[  672.017315] CFG80211-ERROR) wl_scan_timeout : timer expired
[  672.017489] CFG80211-ERROR) wl_escan_handler : WLC_E_STATUS_TIMEOUT : scan_request[f5ab8800]
[  672.017528] CFG80211-ERROR) wl_escan_handler : reason[0xffffffff]
[  672.041560] CFG80211-ERROR) wl_escan_handler : escan is not ready ndev f587d800 drv_status 0x0 e_ty4
[  790.134798] IPv6: wlan0: IPv6 duplicate address fdf8:113:a82b:3a00:7a4b:87ff:fea5:3a73 detected!
```