---
title: Mount NTFS filesystem read/write on Ubuntu

date: 2006-11-29
url: /2006/11/29/mount-ntfs-filesystem-readwrite-on-ubuntu/
categories:
  - Tips and Tricks

---
<img align="left" id="image301" alt="ubuntu logo" src="/uploads/2006/11/ubuntu_logo.gif" />Here is the simple method to enable read write access for your NTFS file system on your Ubuntu Box. This method uses ntfs-3g which is still in beta. You should not use it on production machines.

First enable Universe repository

Then in your terminal type

`sudo apt-get install ntfs-3g`

You can view the partition table by using this command

`sudo fdisk -l`

Then in your /media folder create new mount folders. This is where your filesystem will be mounted. Then make a backup of the /etc/fstab file and edit the file

`sudo mkdir /media/windows<br />
sudo cp /etc/fstab /etc/fstab.bak<br />
gksudo gedit /etc/fstab`
  
Append this line to the fstab file, by substituting the respective drive name. This should be done for every drive in your system.

<pre>/dev/hda1    /media/windows    ntfs-3g    defaults,locale=en_US.utf8    0    0</pre>

Save the file and reboot the system. You can however mount them without reboot by issuing this command.

`sudo umount -a && sudo mount -a`

This would unmount all your file systems and again mount them.