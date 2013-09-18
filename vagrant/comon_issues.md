Common Issues
=============

## VG1

### Components

* Vagrant 1.1
* CentOs 6.4

### Description:

When starting Virtual Machine I got the following
```
The following SSH command responded with a non-zero exit status.
Vagrant assumes that this means the command failed!

/sbin/ifup eth1 2> /dev/null
```
And default shared folder is not mounted


### Solution:

* vagrant ssh
* sudo rm -f /etc/udev/rules.d/70-persistent-net.rule
* vagrant reload
