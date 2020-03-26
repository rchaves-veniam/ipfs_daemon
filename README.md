Folder containing multiple boot scripts, to setup an IPFS repo on flash memory, RAM or SD.

Run from .profile:
```
. /etc/init.d/ipfs_daemon
/etc/init.d/ipfs_daemon start
export EDITOR='vi'
```

TODO: find how to run automatically. Placing it in `/etc/init` with `START=95` doesn't work.