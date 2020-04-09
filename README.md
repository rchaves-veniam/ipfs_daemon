# Description
Folder containing multiple boot scripts, to setup an IPFS repo on flash memory, RAM or SD.

# Mandatory ENV vars:
To choose the IO medium used (TMP,SD, FLASH):
	- `USE_TMP`: if set, the IPFS path will be in `/tmp/ipfs_path`
	- `USE_SD`: if set, the IPFS path will be in `/mnt/mmcblk0p1/ipfs/go-ipfs/.ipfs`, the SD card
	- default: if neither are set, the IPFS path will be in flash, `/root/ipfs_path`

If running in Docker, the DOCKER variable must be set.

# Running from .profile
```
. /etc/init.d/ipfs_daemon
/etc/init.d/ipfs_daemon start
export EDITOR='vi'
```

TODO: find how to run automatically. Placing it in `/etc/init` with `START=95` doesn't work.
