# K9604-W
4ch wireless NVR kit


## NVR
| Param | Value |
| --- | --- |
| Dev name | NVR |
| Dev model	| K9604-W |
| HW version | 2.1.0 |
| SW version | 2.5.0.4_21322230 |
| Reldatetime | 2016/07/05 18:09 |

<details>
  <summary>Click to expand <code>/etc/passwd</code></summary>
  
```bash
# cat /etc/passwd
root:Uu1Kq8MmXhxqA:0:0::/root:/bin/sh
```
</details>

<details>
  <summary>Click to expand <code>/proc/cpuinfo</code></summary>

```bash
# cat /proc/cpuinfo
Processor       : ARMv7 Processor rev 1 (v7l)
BogoMIPS        : 1318.91
Features        : swp half thumb fastmult edsp
CPU implementer : 0x41
CPU architecture: 7
CPU variant     : 0x4
CPU part        : 0xc09
CPU revision    : 1

Hardware        : hi3520d
Revision        : 0000
Serial          : 0000000000000000
```
</details>
<details>
  <summary>Click to expand <code>/proc/mtd</code></summary>

```bash
# cat /proc/mtd
dev:    size   erasesize  name
mtd0: 00080000 00010000 "U"
mtd1: 00040000 00010000 "E"
mtd2: 00040000 00010000 "L"
mtd3: 00080000 00010000 "C"
mtd4: 00280000 00010000 "K"
mtd5: 00c00000 00010000 "R"
```
</details>

<details>
  <summary>Click to expand <code>dmesg</code></summary>
  
```bash
# dmesg
Linux version 3.0.8 (root@archlinux) (gcc version 4.4.1 (Hisilicon_v100(gcc4.4-290+uclibc_0.9.32.1+eabi+linuxpthread)) ) #9 Tue May 24 16:51:50 SGT 2016
CPU: ARMv7 Processor [414fc091] revision 1 (ARMv7), cr=10c53c7f
CPU: VIPT nonaliasing data cache, VIPT aliasing instruction cache
Machine: hi3520d
Memory policy: ECC disabled, Data cache writeback
On node 0 totalpages: 35840
free_area_init_node: node 0, pgdat c0691ac4, node_mem_map c06ef000
  Normal zone: 280 pages used for memmap
  Normal zone: 0 pages reserved
  Normal zone: 35560 pages, LIFO batch:7
pcpu-alloc: s0 r0 d32768 u32768 alloc=1*32768
pcpu-alloc: [0] 0
Built 1 zonelists in Zone order, mobility grouping on.  Total pages: 35560
Kernel command line: mem=140M console=ttyAMA0,115200 root=0100 init=/linuxrc mtdparts=hi_sfc:512K(U),256K(E),256K(L),512K(C),2560K(K),12M(R) ramdisk_size=8000
PID hash table entries: 1024 (order: 0, 4096 bytes)
Dentry cache hash table entries: 32768 (order: 5, 131072 bytes)
Inode-cache hash table entries: 16384 (order: 4, 65536 bytes)
Memory: 140MB = 140MB total
Memory: 127064k/127064k available, 16296k reserved, 0K highmem
Virtual kernel memory layout:
    vector  : 0xffff0000 - 0xffff1000   (   4 kB)
    fixmap  : 0xfff00000 - 0xfffe0000   ( 896 kB)
    DMA     : 0xffc00000 - 0xffe00000   (   2 MB)
    vmalloc : 0xc9000000 - 0xfe000000   ( 848 MB)
    lowmem  : 0xc0000000 - 0xc8c00000   ( 140 MB)
    modules : 0xbf000000 - 0xc0000000   (  16 MB)
      .init : 0xc0008000 - 0xc002f000   ( 156 kB)
      .text : 0xc002f000 - 0xc0662000   (6348 kB)
      .data : 0xc0662000 - 0xc0692140   ( 193 kB)
       .bss : 0xc0692164 - 0xc06eed90   ( 372 kB)
SLUB: Genslabs=13, HWalign=32, Order=0-3, MinObjects=0, CPUs=1, Nodes=1
NR_IRQS:128 nr_irqs:128 128
sched_clock: 32 bits at 82MHz, resolution 12ns, wraps every 52060ms
Console: colour dummy device 80x30
Calibrating delay loop... 1318.91 BogoMIPS (lpj=6594560)
pid_max: default: 32768 minimum: 301
Mount-cache hash table entries: 512
CPU: Testing write buffer coherency: ok
hw perfevents: enabled with ARMv7 Cortex-A9 PMU driver, 7 counters available
devtmpfs: initialized
xor: measuring software checksum speed
   arm4regs  :  1072.000 MB/sec
   8regs     :   802.800 MB/sec
   32regs    :   851.600 MB/sec
xor: using function: arm4regs (1072.000 MB/sec)
NET: Registered protocol family 16
hw-breakpoint: found 6 breakpoint and 1 watchpoint registers.
hw-breakpoint: 1 breakpoint(s) reserved for watchpoint single-step.
hw-breakpoint: maximum watchpoint size is 4 bytes.
Serial: AMBA PL011 UART driver
uart:0: ttyAMA0 at MMIO 0x20080000 (irq = 40) is a PL011 rev2
console [ttyAMA0] enabled
uart:1: ttyAMA1 at MMIO 0x20090000 (irq = 41) is a PL011 rev2
uart:2: ttyAMA2 at MMIO 0x200a0000 (irq = 42) is a PL011 rev2
uart:3: ttyAMA3 at MMIO 0x200b0000 (irq = 43) is a PL011 rev2
bio: create slab <bio-0> at 0
raid6: int32x1     32 MB/s
raid6: int32x2     56 MB/s
raid6: int32x4     75 MB/s
raid6: int32x8    101 MB/s
raid6: using algorithm int32x8 (101 MB/s)
SCSI subsystem initialized
libata version 3.00 loaded.
usbcore: registered new interface driver usbfs
usbcore: registered new interface driver hub
usbcore: registered new device driver usb
cfg80211: Calling CRDA to update world regulatory domain
Switching to clocksource timer1
FS-Cache: Loaded
CacheFiles: Loaded
NET: Registered protocol family 2
IP route cache hash table entries: 2048 (order: 1, 8192 bytes)
TCP established hash table entries: 8192 (order: 4, 65536 bytes)
TCP bind hash table entries: 8192 (order: 3, 32768 bytes)
TCP: Hash tables configured (established 8192 bind 8192)
TCP reno registered
UDP hash table entries: 256 (order: 0, 4096 bytes)
UDP-Lite hash table entries: 256 (order: 0, 4096 bytes)
NET: Registered protocol family 1
RPC: Registered named UNIX socket transport module.
RPC: Registered udp transport module.
RPC: Registered tcp transport module.
RPC: Registered tcp NFSv4.1 backchannel transport module.
Trying to unpack rootfs image as initramfs...
rootfs image is not initramfs (junk in compressed archive); looks like an initrd
Freeing initrd memory: 7828K
NetWinder Floating Point Emulator V0.97 (double precision)
L2cache cache controller enabled
VFS: Disk quotas dquot_6.5.2
Dquot-cache hash table entries: 1024 (order 0, 4096 bytes)
DLM installed
squashfs: version 4.0 (2009/01/31) Phillip Lougher
NTFS driver 2.1.30 [Flags: R/W].
fuse init (API version 7.16)
SGI XFS with security attributes, large block/inode numbers, no debug enabled
msgmni has been set to 263
alg: No test for stdrng (krng)
Block layer SCSI generic (bsg) driver version 0.4 loaded (major 254)
io scheduler noop registered
io scheduler deadline registered (default)
io scheduler cfq registered
brd: module loaded
loop: module loaded
Loading iSCSI transport class v2.0-870.
SCSI Media Changer driver v0.25
ahci: SSS flag set, parallel bus scan disabled
ahci ahci.0: AHCI 0001.0200 32 slots 2 ports 3 Gbps 0x3 impl platform mode
ahci ahci.0: flags: ncq sntf stag pm led clo only pmp pio slum part ccc sxs boh
scsi0 : ahci_platform
scsi1 : ahci_platform
ata1: SATA max UDMA/133 mmio [mem 0x10080000-0x1008ffff] port 0x100 irq 52
ata2: SATA max UDMA/133 mmio [mem 0x10080000-0x1008ffff] port 0x180 irq 52
Spi id table Version 1.22
Hisilicon Spi Flash Controller V350 Device Driver, Version 1.10
Spi(cs1) ID: 0xC2 0x20 0x18 0xC2 0x20 0x18
SPI FLASH start_up_mode is 3 Bytes
Spi(cs1):
Block:64KB
Chip:16MB
Name:"MX25L128XX"
spi size: 16MB
chip num: 1
6 cmdlinepart partitions found on MTD device hi_sfc
Creating 6 MTD partitions on "hi_sfc":
0x000000000000-0x000000080000 : "U"
0x000000080000-0x0000000c0000 : "E"
0x0000000c0000-0x000000100000 : "L"
0x000000100000-0x000000180000 : "C"
0x000000180000-0x000000400000 : "K"
0x000000400000-0x000001000000 : "R"
Fixed MDIO Bus: probed
himii: probed
Invalid HW-MAC Address: 00:00:00:00:00:00
Set Random MAC address: F2:EA:22:2D:3D:B0
bonding: Ethernet Channel Bonding Driver: v3.7.1 (April 27, 2011)
bonding: Warning: either miimon or arp_interval and arp_ip_target module parameters must be specified, otherwise bonding will not detect link failures! see bonding.txt for details.
PPP generic driver version 2.4.2
PPP Deflate Compression module registered
PPP BSD Compression module registered
PPP MPPE Compression module registered
NET: Registered protocol family 24
SLIP: version 0.8.4-NET3.019-NEWTTY (dynamic channels, max=256).
CSLIP: code copyright 1989 Regents of the University of California.
SLIP linefill/keepalive option.
usbmon: debugfs is not available
ehci_hcd: USB 2.0 'Enhanced' Host Controller (EHCI) Driver
hiusb-ehci hiusb-ehci.0: HIUSB EHCI
hiusb-ehci hiusb-ehci.0: new USB bus registered, assigned bus number 1
hiusb-ehci hiusb-ehci.0: irq 53, io mem 0x100b0000
hiusb-ehci hiusb-ehci.0: USB 0.0 started, EHCI 1.00
hub 1-0:1.0: USB hub found
hub 1-0:1.0: 2 ports detected
ohci_hcd: USB 1.1 'Open' Host Controller (OHCI) Driver
hiusb-ohci hiusb-ohci.0: HIUSB OHCI
hiusb-ohci hiusb-ohci.0: new USB bus registered, assigned bus number 2
hiusb-ohci hiusb-ohci.0: irq 54, io mem 0x100a0000
hub 2-0:1.0: USB hub found
hub 2-0:1.0: 2 ports detected
usbcore: registered new interface driver cdc_acm
cdc_acm: USB Abstract Control Model driver for USB modems and ISDN adapters
Initializing USB Mass Storage driver...
usbcore: registered new interface driver usb-storage
USB Mass Storage support registered.
usbcore: registered new interface driver ums-alauda
usbcore: registered new interface driver ums-cypress
usbcore: registered new interface driver ums-datafab
usbcore: registered new interface driver ums_eneub6250
usbcore: registered new interface driver ums-freecom
usbcore: registered new interface driver ums-isd200
usbcore: registered new interface driver ums-jumpshot
usbcore: registered new interface driver ums-karma
usbcore: registered new interface driver ums-onetouch
usbcore: registered new interface driver ums-realtek
usbcore: registered new interface driver ums-sddr09
usbcore: registered new interface driver ums-sddr55
usbcore: registered new interface driver ums-usbat
usbcore: registered new interface driver usbserial
USB Serial support registered for generic
usbcore: registered new interface driver usbserial_generic
usbserial: USB Serial Driver core
USB Serial support registered for GSM modem (1-port)
usbcore: registered new interface driver option
option: v0.7.2:USB Driver for GSM modems
mousedev: PS/2 mouse device common for all mice
md: linear personality registered for level -1
md: raid0 personality registered for level 0
md: raid1 personality registered for level 1
md: raid10 personality registered for level 10
md: raid6 personality registered for level 6
md: raid5 personality registered for level 5
md: raid4 personality registered for level 4
md: multipath personality registered for level -4
md: faulty personality registered for level -5
device-mapper: ioctl: 4.20.0-ioctl (2011-02-02) initialised: dm-devel@redhat.com
device-mapper: multipath: version 1.3.0 loaded
device-mapper: multipath round-robin: version 1.0.0 loaded
device-mapper: multipath queue-length: version 0.1.0 loaded
device-mapper: multipath service-time: version 0.2.0 loaded
device-mapper: dm-log-userspace: version 1.1.0 loaded
usbcore: registered new interface driver usbhid
usbhid: USB HID core driver
TCP cubic registered
Initializing XFRM netlink socket
NET: Registered protocol family 10
IPv6 over IPv4 tunneling driver
NET: Registered protocol family 17
NET: Registered protocol family 15
802.1Q VLAN Support v1.8
sctp: Hash tables configured (established 4096 bind 8192)
lib80211: common routines for IEEE802.11 drivers
lib80211_crypt: registered algorithm 'NULL'
lib80211_crypt: registered algorithm 'WEP'
lib80211_crypt: registered algorithm 'CCMP'
lib80211_crypt: registered algorithm 'TKIP'
usb 1-2: new high speed USB device number 2 using hiusb-ehci
ata1: SATA link up 1.5 Gbps (SStatus 113 SControl 300)
ata1.00: ATA-8: Hitachi HUA722020ALA331, JKAOA3NH, max UDMA/133
ata1.00: 3907029168 sectors, multi 0: LBA48 NCQ (depth 31/32)
ata1.00: configured for UDMA/133
scsi 0:0:0:0: Direct-Access     ATA      Hitachi HUA72202 JKAO PQ: 0 ANSI: 5
sd 0:0:0:0: [sda] 3907029168 512-byte logical blocks: (2.00 TB/1.81 TiB)
sd 0:0:0:0: [sda] Write Protect is off
sd 0:0:0:0: [sda] Mode Sense: 00 3a 00 00
sd 0:0:0:0: Attached scsi generic sg0 type 0
sd 0:0:0:0: [sda] Write cache: enabled, read cache: enabled, doesn't support DPO or FUA
 sda: sda1 sda2
sd 0:0:0:0: [sda] Attached SCSI disk
ata2: SATA link down (SStatus 0 SControl 300)
md: Waiting for all devices to be available before autodetect
md: If you don't use raid, use raid=noautodetect
md: Autodetecting RAID arrays.
md: Scanned 0 and added 0 devices.
md: autorun ...
md: ... autorun DONE.
RAMDISK: squashfs filesystem found at block 0
RAMDISK: Loading 7825KiB [1 disk] into ram disk... done.
VFS: Mounted root (squashfs filesystem) readonly on device 1:0.
devtmpfs: mounted
Freeing init memory: 156K
udevd (700): /proc/700/oom_adj is deprecated, please use /proc/700/oom_score_adj instead.
ADDRCONF(NETDEV_UP): eth0: link is not ready
PHY: himii:03 - Link is Up - 100/Full
ADDRCONF(NETDEV_CHANGE): eth0: link becomes ready
Hisilicon Media Memory Zone Manager
hi3520D_base: module license 'Proprietary' taints kernel.
Disabling lock debugging due to kernel taint
Hisilicon UMAP device driver interface: v3.00
load sys.ko ...OK!
Load tde.ko ...OK!
load venc.ko ...OK!
load group.ko ...OK!
load chnl.ko ...OK!
load h264e.ko ...OK!
load rc.ko ...OK!
load jpege.ko ...OK!
load viu.ko ...OK!
load vou.ko ....OK!
load vpss.ko ....OK!
load vda.ko ....OK!
load region.ko ....OK!
load vdec.ko ....OK
load vhd firmware.ko OK
load hdmi.ko ....OK!
Load jpeg6b.ko success.         (SDK_VERSION:[jpeg6bv1.0] Build Time:[Sep 29 2014, 18:04:52])
Hisilicon Watchdog Timer: 0.01 initialized. default_margin=60 sec (nowayout= 0, nodeamon= 1)
HI3515 base @ 18:09:35 Jul  5 2016
GPIO I2C for HI35xx @ 18:09:35 Jul  5 2016
GPIO_MODE:RMII disable
tmpClkV=0x002547ae
GPIO_MODE:GPIO_PLAT_TYPE8
PERI_CRG_REG51:addr=0x200300cc, val=0x00000002
IO_CONFIG_REG(38):addr=0x200f0098, val=0x00000000
IO_CONFIG_REG(39):addr=0x200f009c, val=0x00000000
IO_CONFIG_REG(40):addr=0x200f00a0, val=0x00000000
IO_CONFIG_REG(41):addr=0x200f00a4, val=0x00000000
IO_CONFIG_REG(42):addr=0x200f00a8, val=0x00000000
IO_CONFIG_REG(43):addr=0x200f00ac, val=0x00000000
IO_CONFIG_REG(44):addr=0x200f00b0, val=0x00000000
IO_CONFIG_REG(45):addr=0x200f00b4, val=0x00000000
IO_CONFIG_REG(46):addr=0x200f00b8, val=0x00000001
IO_CONFIG_REG(47):addr=0x200f00bc, val=0x00000001
IO_CONFIG_REG(48):addr=0x200f00c0, val=0x00000000
IO_CONFIG_REG(49):addr=0x200f00c4, val=0x00000000
IO_CONFIG_REG(50):addr=0x200f00c8, val=0x00000000
GPIO Init Succeed!
input: keypad as /devices/virtual/input/input0
Keypad for HI3515 @ 18:09:35 Jul  5 2016
input: irda as /devices/virtual/input/input1
Irda for HI3515 @ 18:09:35 Jul  5 2016
RTL871X: module init start
RTL871X: rtl8188eu v4.3.0.6_12167.20150923
RTL871X: build time: May 17 2016 11:27:06
bFWReady == _FALSE call reset 8051...
RTL871X: rtw_ndev_init(wlan0)
usbcore: registered new interface driver rtl8188eu
RTL871X: module init ret=0
eth0: no IPv6 routers present
==> rtl8188e_iol_efuse_patch
ADDRCONF(NETDEV_UP): wlan0: link is not ready
RTL871X: set group key camid:1, addr:00:00:00:00:00:00, kid:1, type:AES
RTL871X: assoc success
ADDRCONF(NETDEV_CHANGE): wlan0: link becomes ready
ADDRCONF(NETDEV_UP): eth0: link is not ready
PHY: himii:03 - Link is Up - 100/Full
ADDRCONF(NETDEV_CHANGE): eth0: link becomes ready
input: keypad as /devices/virtual/input/input2
Keypad for HI3515 @ 18:09:35 Jul  5 2016
ES8323 driver v1.00.017,build time:Jul  5 2016 18:09:36
Es8323_postphone_init:begin
Es8323_postphone_init:audio codec not exist!
Es8323_postphone_init:end
[Es8323_ioctl, 596]: Unsupported Cmd -2147204856
[Es8323_ioctl, 596]: Unsupported Cmd 1074020609
[Es8323_ioctl, 596]: Unsupported Cmd 16651
wlan0: no IPv6 routers present
EXT3-fs: barriers not enabled
kjournald starting.  Commit interval 5 seconds
EXT3-fs (sda1): using internal journal
EXT3-fs (sda1): mounted filesystem with ordered data mode
eth0: no IPv6 routers present
kjournald starting.  Commit interval 5 seconds
EXT3-fs (sda1): using internal journal
EXT3-fs (sda1): mounted filesystem with ordered data mode
RTL871X: ERROR rtw_hal_macid_wakeup(wlan0): Invalid macid(32)
RTL871X: ERROR rtw_hal_macid_wakeup(wlan0): Invalid macid(32)
RTL871X: indicate disassoc
ADDRCONF(NETDEV_UP): wlan0: link is not ready
RTL871X: set group key camid:1, addr:00:00:00:00:00:00, kid:1, type:AES
RTL871X: assoc success
ADDRCONF(NETDEV_CHANGE): wlan0: link becomes ready
wlan0: no IPv6 routers present
RTL871X: set group key camid:1, addr:00:00:00:00:00:00, kid:1, type:TKIP
RTL871X: assoc success
```
</details>




## Camera

| Param | Value |
| --- | --- |
|Device Name	| ip-camera |
|Device Model | IPC |
|Hardware Version	| 1.3.0. |
|Software Version	| 1.7.5.57801024 |
|Release Time	| 2016/08/12 10:55:40 |

<details>
  <summary>Click to expand <code>/etc/passwd</code></summary>
  
```bash
# cat /etc/passwd
root:Uu1Kq8MmXhxqA:0:0::/root:/bin/sh
```
</details>

<details>
  <summary>Click to expand <code>/proc/cpuinfo</code></summary>

```bash
# cat /proc/cpuinfo
Processor       : ARM926EJ-S rev 5 (v5l)
BogoMIPS        : 269.10
Features        : swp half thumb fastmult edsp java
CPU implementer : 0x41
CPU architecture: 5TEJ
CPU variant     : 0x0
CPU part        : 0x926
CPU revision    : 5

Hardware        : hi3518ev200
Revision        : 0000
Serial          : 0000000000000000
```
</details>
<details>
  <summary>Click to expand <code>/proc/mtd</code></summary>

```bash
# cat /proc/mtd
dev:    size   erasesize  name
mtd0: 00030000 00010000 "uboot"
mtd1: 00010000 00010000 "env"
mtd2: 00010000 00010000 "user"
mtd3: 00060000 00010000 "conf"
mtd4: 001e0000 00010000 "kernel"
mtd5: 003f0000 00010000 "rootfs"
mtd6: 00180000 00010000 "custom"
```
</details>

<details>
  <summary>Click to expand <code>dmesg</code></summary>
  
```bash
# dmesg
Booting Linux on physical CPU 0
Linux version 3.4.35 (root@green-VM) (gcc version 4.8.3 20131202 (prerelease) (Hisilicon_v300) ) #14 Mon Oct 12 10:04:04 CST 2015
CPU: ARM926EJ-S [41069265] revision 5 (ARMv5TEJ), cr=00053177
CPU: VIVT data cache, VIVT instruction cache
Machine: hi3518ev200
Memory policy: ECC disabled, Data cache writeback
On node 0 totalpages: 10240
free_area_init_node: node 0, pgdat c04f532c, node_mem_map c0534000
  Normal zone: 80 pages used for memmap
  Normal zone: 0 pages reserved
  Normal zone: 10160 pages, LIFO batch:1
pcpu-alloc: s0 r0 d32768 u32768 alloc=1*32768
pcpu-alloc: [0] 0
Built 1 zonelists in Zone order, mobility grouping on.  Total pages: 10160
Kernel command line: mem=40M console=ttyAMA0,115200 root=0100 init=/linuxrc mtdparts=hi_sfc:192K(uboot),64K(env),64K(user),384K(conf),1920K(kernel),4032K(rootfs),1536K(custom) ramdisk_size=3904
PID hash table entries: 256 (order: -2, 1024 bytes)
Dentry cache hash table entries: 8192 (order: 3, 32768 bytes)
Inode-cache hash table entries: 4096 (order: 2, 16384 bytes)
Memory: 40MB = 40MB total
Memory: 31568k/31568k available, 9392k reserved, 0K highmem
Virtual kernel memory layout:
    vector  : 0xffff0000 - 0xffff1000   (   4 kB)
    fixmap  : 0xfff00000 - 0xfffe0000   ( 896 kB)
    vmalloc : 0xc3000000 - 0xff000000   ( 960 MB)
    lowmem  : 0xc0000000 - 0xc2800000   (  40 MB)
    modules : 0xbf000000 - 0xc0000000   (  16 MB)
      .text : 0xc0008000 - 0xc04aa000   (4744 kB)
      .init : 0xc04aa000 - 0xc04cb1dc   ( 133 kB)
      .data : 0xc04cc000 - 0xc04f5a60   ( 167 kB)
       .bss : 0xc04f5a84 - 0xc0533438   ( 247 kB)
SLUB: Genslabs=13, HWalign=32, Order=0-3, MinObjects=0, CPUs=1, Nodes=1
NR_IRQS:32
VIC @fe0d0000: id 0x00641190, vendor 0x41
sched_clock: 32 bits at 49MHz, resolution 20ns, wraps every 86767ms
Console: colour dummy device 80x30
Calibrating delay loop... 269.10 BogoMIPS (lpj=1345536)
pid_max: default: 32768 minimum: 301
Mount-cache hash table entries: 512
Initializing cgroup subsys freezer
CPU: Testing write buffer coherency: ok
Setting up static identity map for 0x803928e8 - 0x80392940
dummy:
NET: Registered protocol family 16
Serial: AMBA PL011 UART driver
uart:0: ttyAMA0 at MMIO 0x20080000 (irq = 5) is a PL011 rev2
console [ttyAMA0] enabled
uart:1: ttyAMA1 at MMIO 0x20090000 (irq = 30) is a PL011 rev2
uart:2: ttyAMA2 at MMIO 0x200a0000 (irq = 25) is a PL011 rev2
bio: create slab <bio-0> at 0
SCSI subsystem initialized
hi-spi-master hi-spi-master.0: with 1 chip select slaves attached
hi-spi-master hi-spi-master.1: with 2 chip select slaves attached
usbcore: registered new interface driver usbfs
usbcore: registered new interface driver hub
usbcore: registered new device driver usb
cfg80211: Calling CRDA to update world regulatory domain
Switching to clocksource timer0
FS-Cache: Loaded
CacheFiles: Loaded
NET: Registered protocol family 2
IP route cache hash table entries: 1024 (order: 0, 4096 bytes)
TCP established hash table entries: 2048 (order: 2, 16384 bytes)
TCP bind hash table entries: 2048 (order: 1, 8192 bytes)
TCP: Hash tables configured (established 2048 bind 2048)
TCP: reno registered
UDP hash table entries: 256 (order: 0, 4096 bytes)
UDP-Lite hash table entries: 256 (order: 0, 4096 bytes)
NET: Registered protocol family 1
RPC: Registered named UNIX socket transport module.
RPC: Registered udp transport module.
RPC: Registered tcp transport module.
RPC: Registered tcp NFSv4.1 backchannel transport module.
Trying to unpack rootfs image as initramfs...
rootfs image is not initramfs (junk in compressed archive); looks like an initrd
Freeing initrd memory: 3644K
VFS: Disk quotas dquot_6.5.2
Dquot-cache hash table entries: 1024 (order 0, 4096 bytes)
squashfs: version 4.0 (2009/01/31) Phillip Lougher
NFS: Registering the id_resolver key type
jffs2: version 2.2. (NAND) © 2001-2006 Red Hat, Inc.
ROMFS MTD (C) 2007 Red Hat, Inc.
fuse init (API version 7.18)
msgmni has been set to 68
Block layer SCSI generic (bsg) driver version 0.4 loaded (major 254)
io scheduler noop registered
io scheduler deadline registered (default)
io scheduler cfq registered
brd: module loaded
loop: module loaded
SPI Nor(cs 0) ID: 0xc2 0x20 0x17
SPI(cs0):
Block:64KB
Chip:8MB
Name:"MX25L6406E"
7 cmdlinepart partitions found on MTD device hi_sfc
7 cmdlinepart partitions found on MTD device hi_sfc
Creating 7 MTD partitions on "hi_sfc":
0x000000000000-0x000000030000 : "uboot"
0x000000030000-0x000000040000 : "env"
0x000000040000-0x000000050000 : "user"
0x000000050000-0x0000000b0000 : "conf"
0x0000000b0000-0x000000290000 : "kernel"
0x000000290000-0x000000680000 : "rootfs"
0x000000680000-0x000000800000 : "custom"
himii: probed
ehci_hcd: USB 2.0 'Enhanced' Host Controller (EHCI) Driver
hiusb-ehci hiusb-ehci.0: HIUSB EHCI
hiusb-ehci hiusb-ehci.0: new USB bus registered, assigned bus number 1
hiusb-ehci hiusb-ehci.0: irq 15, io mem 0x100b0000
hiusb-ehci hiusb-ehci.0: USB 0.0 started, EHCI 1.00
hub 1-0:1.0: USB hub found
hub 1-0:1.0: 1 port detected
ohci_hcd: USB 1.1 'Open' Host Controller (OHCI) Driver
hiusb-ohci hiusb-ohci.0: HIUSB OHCI
hiusb-ohci hiusb-ohci.0: new USB bus registered, assigned bus number 2
hiusb-ohci hiusb-ohci.0: irq 16, io mem 0x100a0000
hub 2-0:1.0: USB hub found
hub 2-0:1.0: 1 port detected
Initializing USB Mass Storage driver...
usbcore: registered new interface driver usb-storage
USB Mass Storage support registered.
dwc_otg: version 3.00a 10-AUG-2012
Core Release: 3.10a
Setting default values for core params
Using Buffer DMA mode
Periodic Transfer Interrupt Enhancement - disabled
Multiprocessor Interrupt Enhancement - disabled
OTG VER PARAM: 0, OTG VER FLAG: 0
Dedicated Tx FIFOs mode
i2c /dev entries driver
hisi_i2c hisi_i2c.0: Hisilicon [i2c-0] probed!
hisi_i2c hisi_i2c.1: Hisilicon [i2c-1] probed!
hisi_i2c hisi_i2c.2: Hisilicon [i2c-2] probed!
usb 1-1: new high-speed USB device number 2 using hiusb-ehci
TCP: bic registered
TCP: cubic registered
TCP: westwood registered
TCP: htcp registered
Initializing XFRM netlink socket
NET: Registered protocol family 17
NET: Registered protocol family 15
8021q: 802.1Q VLAN Support v1.8
lib80211: common routines for IEEE802.11 drivers
lib80211_crypt: registered algorithm 'NULL'
lib80211_crypt: registered algorithm 'WEP'
lib80211_crypt: registered algorithm 'CCMP'
lib80211_crypt: registered algorithm 'TKIP'
Registering the dns_resolver key type
RAMDISK: squashfs filesystem found at block 0
RAMDISK: Loading 3641KiB [1 disk] into ram disk... done.
VFS: Mounted root (squashfs filesystem) readonly on device 1:0.
Freeing init memory: 132K
Hisilicon Media Memory Zone Manager
Module himedia: init ok
hi3518e_base: module license 'Proprietary' taints kernel.
Disabling lock debugging due to kernel taint
load sys.ko for Hi3518EV200...OK!
load tde.ko ...OK!
load region.ko ....OK!
load vgs.ko for Hi3518EV200...OK!
ISP Mod init!
load viu.ko for Hi3518EV200...OK!
load vpss.ko ....OK!
load rc.ko for Hi3518EV200...OK!
load venc.ko for Hi3518EV200...OK!
load chnl.ko for Hi3518EV200...OK!
load h264e.ko for Hi3518EV200...OK!
load jpege.ko for Hi3518EV200...OK!
PHY: himii:01 - Link is Up - 100/Full
load ive.ko for Hi3518EV200...OK!
JUAN Watchdog Timer: 0.01 initialized. default_margin=60 sec (nowayout= 0, nodeamon= 0)
acodec inited!
mipi_init
init phy power successful!
load hi_mipi driver successful!
hi_i2c init is ok!
RTL871X: module init start
RTL871X: rtl8188eu v4.3.24_16705.20160509
RTL871X: build time: Jun 18 2016 17:39:00
bFWReady == _FALSE call reset 8051...
RTL871X: hal_com_config_channel_plan chplan:0x23
RTL871X: rtw_ndev_init(wlan0) if1 mac_addr=[mac_addr]
RTL871X: rtw_ndev_init(wlan1) if2 mac_addr=[mac_addr]
usbcore: registered new interface driver rtl8188eu
RTL871X: module init ret=0
==> rtl8188e_iol_efuse_patch
RTL871X: indicate disassoc
***link down status changed***.
PHY: himii:01 - Link is Down
PHY: himii:01 - Link is Up - 100/Full
RTL871X: set group key camid:1, addr:00:00:00:00:00:00, kid:1, type:AES
RTL871X: assoc success

```
</details>
