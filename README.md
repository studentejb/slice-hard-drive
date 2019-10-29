# slice-hard-drive
disk partioning
check drives
 #lsblk
 partioning drives
 #fdisk /dev/sdb
 adding file system
 #mkfs.ext4 /dev/sdb1
 create mount point directory i cd to root
 #mkdir /mountpoint
 #mount -t ext4 /dev/sdb1 /mountpoint
 check mount point
 #df -h
 fix kernel mount
 #vi /etc/fstab
 /dev/sdb1 /mountpoint ext4 defaults 0 0
 save
 check kernel mount
 #mount -a
