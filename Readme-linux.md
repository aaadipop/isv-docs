## Linux cheat sheet

1. Display information about the operating system distribution

    ```bash
    cat /etc/os-release
    ```
   
2. Edit filename starting at line 1

    ```bash
    vi filename	 
    ```
   
3. **i** - insert text before cursor, until <Esc> hit
4. **:wq<Return>** - quit vi, writing out modified file to file named in original invocation

5. Start Nginx service

    ```bash
    sudo service nginx start	 
    ```

6. Check Nginx service status

    ```bash
    sudo service nginx status	
    ```

7. Grow partition
https://zebrahost.com/docs/centos/resizing-disk-in-centos-7/
```
Grow disk on snak
sda/sda2-centos-root
/dev/mapper/centos-root

lsblk
fdisk -l
fdisk /dev/sda
partprobe /dev/sda
lsblk
pvresize /dev/sda2
lvresize /dev/mapper/centos-root /dev/sda2
resize2fs /dev/mapper/centos-root
xfs_growfs /dev/centos/root
df -h

Grow disk on ns1
sda/sda2-centos_ns2-home
/dev/mapper/centos_ns2-home

lsblk
fdisk -l
fdisk /dev/sda
partprobe /dev/sda
lsblk
pvresize /dev/sda2
lvresize /dev/mapper/centos_ns2-home /dev/sda2
resize2fs /dev/mapper/centos_ns2-home
file -sL /dev/centos_ns2/home
xfs_growfs /dev/centos_ns2/home
df -h

```