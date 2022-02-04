# OpenSUSE MicroOS combustion

I have created a combustion usb for MicroOS

Create a ssh key with the name server. Copy the content of the file server.pub to the server.pub file in this directory.

Default password for the user server is:
12345

## Create USB

To create the USB use this code
```
mkfs.ext4 /dev/sdY
e2label /dev/sdY combustion
mount /dev/sdY /mnt
cd /mnt
git clone https://github.com/SolidRhino/openSUSE-MicroOS.git combustion
```