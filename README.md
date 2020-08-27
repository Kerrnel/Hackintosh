# Ackintosh

<H3>Latest CLOVER folders for</H3>

```
ASRock H370-itx
ASRock Z390-itx
ASMini 300W
Hystou 7500
Hystou 8500
NUC8 i7
Gigabyte Brix i5
Gigabyte Brix i7
```

```
BTRFS Note - 
	UEFI FS drivers https://efi.akeo.ie/downloads/efifs-latest/x64/
		Or from latest refind build (good to install anyway)
	Volume - select it in Clover Configurator
		Use mkfs.btrfs -L MyName /dev/xyz
	Or use PARTUUID
		From blkid on Linux
		Or diskutil info disk0sX on macOS

	One can install as many Linux distros as fit on disk in one btrfs
	volume; therefore I use subvolumes:
		System/Debian
		System/Ubuntu
			... etc
		Users (/home)
		Applications (/opt, /usr/local)
		Library (common scripts, configs, binaries for all - I mount in /all)
		Cache (can throw whatever away - /var/tmp, /var/cache)
		Variable (other common /var directories like /var/mail)
```

Latest OS - Catalina 10.15.2
