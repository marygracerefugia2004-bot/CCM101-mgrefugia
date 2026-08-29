# Infrastructure Report

## Linux Server Investigation

The Linux environment was checked using the KillerCoda terminal. The commands were used to get the system and server information.

## System Information

| Information         | Result                                        |
| ------------------- | --------------------------------------------- |
| Operating System    | Ubuntu 24.04.4 LTS (Noble Numbat)             |
| Kernel Version      | 6.8.0-138-generic                             |
| CPU Model           | Intel Xeon E312xx (Sandy Bridge, IBRS update) |
| Number of CPU Cores | 1                                             |
| Total RAM           | 1.9Gi                                         |
| Disk Capacity       | 19G                                           |
| Hostname            | ubuntu                                        |
| IP Address          | 172.30.1.2, 172.17.0.1                        |

## Mounted File Systems

These are the mounted file systems shown by `df -h`.

| Filesystem | Size | Used | Avail | Mounted on |
| ---------- | ---: | ---: | ----: | ---------- |
| tmpfs      | 191M | 996K |  190M | /run       |
| /dev/vda1  |  19G | 5.4G |   13G | /          |
| tmpfs      | 952M |  84K |  952M | /dev/shm   |
| tmpfs      | 5.0M |    0 |  5.0M | /run/lock  |
| /dev/vda16 | 881M | 117M |  703M | /boot      |
| /dev/vda15 | 105M | 6.2M |   99M | /boot/efi  |

## Linux Commands Used

These commands were used to get the information:

```bash
cat /etc/os-release
uname -r
lscpu
free -h
df -h
hostname
hostname -I
```

## Summary

The server uses Ubuntu 24.04.4 LTS. It has 1 CPU core, 1.9Gi of RAM, and a 19G disk. The hostname, IP address, and mounted file systems were also identified.
