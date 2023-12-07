# Odyssey- STM32Mp135D- SDCARD image

SDCard image file, was generated following the Buildroot process for the STM32MP135D SBC 
detailed here; 

https://wiki.seeedstudio.com/ODYSSEY-STM32MP135D/

This Repo only hosts the SDcard image for the STM32MP135D SBC as I know it works. 

Make sure you format your SDCard on a linux machine, formatting the SDCard in windows never worked.
We used the Disks tool in Mint to format the SDcard (32GB) 

It generated 2x1MB 1x4MB 1x2MB and 1x60MB partitions when the following command is run: 

sudo dd if=output/images/sdcard.img of=/dev/sdX bs=4M conv=fsync

Where sdX corresponds to the micro sd card device node ... use 'lsblk' command to determine node.





