# Disk management

## General commands

### List disks

```
$ lsblk
```

## Disk partition & format

### Create partition

```
$ fdisk /dev/sdb
```

### Format disk ext4

```
$ mkfs.ext4 /dev/sdb1
```

## Write on removed clusters

### Shred disk

```
$ shred -vf /dev/sdc
```

### DD disk with urandom

```
dd if=/dev/urandom of=/dev/sdb bs=10
```
