# linuxcourse

Relative Path Vs obsolute path.
(.., ~)


#File system infor
xfs_io -x -c "resblks" /
xfs_info /


#LVM Creation
dnf install lvm
lsblk
fdisk -l
pvcreate /dev/xvdf
pvs
vgcreate data /dev/xvdf
vgs
lvcreate -n datalv -L 2G data
mkfs -t xfs /dev/data/datalv
vi /etc/fstab
/dev/data/datalv /test defaults 0 0 
  
#swap creation
 mkswap /dev/xvdg1
 vi /etc/fstab
 swapon -a
 cat /proc/swaps
 free -g
  
  
  
  
  
  
