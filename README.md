BBBOverlay
==========
Working overlay for W1 Bus, on Pin 9_15
To install :copy file to /lib/firmware

To check: echo BB-W1RK > /sys/devices/bone_capemgr.9/slots
Run dmesg to see if there were notrouble

To install at startup:
mount /dev/mmcblk0p1 /mnt/boot
cd /mnt/boot
vim  uEnv.txt
add BB-W1RK to _partno=BB-UART1,BB-W1RK
