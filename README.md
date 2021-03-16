# memory
* https://www.binarytides.com/linux-command-check-memory-usage/

free -m
```
              total       utilisé      libre     partagé tamp/cache   disponible
Mem:           3857        1656         952          46        1248        1881
Partition d'échange:        6674        3292        3382

top

htop
```

vmstat  -s
```
      3949716 K mémoire totale
      1695492 K mémoire utilisée
       985144 K mémoire active
       833696 K mémoire inactive
       975716 K mémoire libre
       375284 K mémoire tampon
       903224 K mémoire échange
      6835196 K échange total
      3371244 K échange utilisé
      3463952 K partition d'échange libre
      4229557 tics du cpu utilisateur non-courtois
        61671 tics cpu utilisateur courtois
      2822083 tics cpu système
    280580028 tics cpu inactif
       608107 tics cpu attente E/S
            0 tics cpu IRQ
        25136 tics cpu IRQ soft
            0 tics cpu volés
    132461602 pages lues depuis le disque
    114959153 pages écrites sur le disque
       163899 pages mises en mémoire d'échange
       951298 pages sorties de la mémoire d'échange
    368020885 interruptions
    769079857 changements de contexte CPU
   1613503944 heure d'amorçage
      2467217 clonages
```

cat /proc/meminfo
```
MemTotal:        3949716 kB
MemFree:          975056 kB
MemAvailable:    1925868 kB
Buffers:          375232 kB
Cached:           766976 kB
SwapCached:        88284 kB
Active:           985064 kB
Inactive:         833664 kB
Active(anon):     360532 kB
Inactive(anon):   368188 kB
Active(file):     624532 kB
Inactive(file):   465476 kB
Unevictable:       11652 kB
Mlocked:           11652 kB
SwapTotal:       6835196 kB
SwapFree:        3463952 kB
Dirty:               360 kB
Writeback:             0 kB
AnonPages:        662576 kB
Mapped:           227220 kB
Shmem:             47708 kB
Slab:             285776 kB
SReclaimable:     136188 kB
SUnreclaim:       149588 kB
KernelStack:       10112 kB
PageTables:        71440 kB
NFS_Unstable:          0 kB
Bounce:                0 kB
WritebackTmp:          0 kB
CommitLimit:     8810052 kB
Committed_AS:    8627576 kB
VmallocTotal:   34359738367 kB
VmallocUsed:           0 kB
VmallocChunk:          0 kB
HardwareCorrupted:     0 kB
AnonHugePages:         0 kB
ShmemHugePages:        0 kB
ShmemPmdMapped:        0 kB
CmaTotal:              0 kB
CmaFree:               0 kB
HugePages_Total:       0
HugePages_Free:        0
HugePages_Rsvd:        0
HugePages_Surp:        0
Hugepagesize:       2048 kB
DirectMap4k:     1831928 kB
DirectMap2M:     2273280 kB
```

sudo dmidecode -t 17
```
# dmidecode 3.1
Getting SMBIOS data from sysfs.
SMBIOS 2.4 present.

Handle 0x0016, DMI type 17, 27 bytes
Memory Device
	Array Handle: 0x0014
	Error Information Handle: No Error
	Total Width: Unknown
	Data Width: Unknown
	Size: 2048 MB
	Form Factor: SODIMM
	Set: None
	Locator: DIMM0
	Bank Locator: BANK 0
	Type: DDR3
	Type Detail: Synchronous
	Speed: 1333 MT/s
	Manufacturer: 0x80AD
	Serial Number: 0x25C2555F
	Asset Tag: Unknown
	Part Number: 0x484D54333235533642465238432D48392020

Handle 0x0017, DMI type 17, 27 bytes
Memory Device
	Array Handle: 0x0014
	Error Information Handle: No Error
	Total Width: Unknown
	Data Width: Unknown
	Size: No Module Installed
	Form Factor: SODIMM
	Set: None
	Locator: DIMM0
	Bank Locator: BANK 1
	Type: Unknown
	Type Detail: None
	Speed: Unknown
	Manufacturer: Not Specified
	Serial Number: Not Specified
	Asset Tag: Unknown
	Part Number: Not Specified

```
