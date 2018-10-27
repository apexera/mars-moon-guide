============================================
Firmware Upgrade
============================================

NetBot supports upgrade in both Uboot and System environments. 


UBoot Upgrade
============================================

Upgrading in u-boot is relative complex, and we have about 5 kinds of methods. 

Before upgrading, we need to prepare the upgrading environment:

1. Prepare the serial debug adapter (**ttl** instead of rs232) 
2. Install serial tool:

    * ``secureCRT`` or ``xshell`` for windows host.
    * ``minicom`` for linux host.
3. Config serial tool for the serial port with following parameters:

   * Baud rate: 57600
   * Data bit: 8
   * Stop bit: 1
   * Parity check: none
   * Flow control: none
4. 

UBoot Upgrade with TFTP
----------------------------------------------------


UBoot Upgrade with SD Disk
----------------------------------------------------


UBoot Upgrade with USB Disk
----------------------------------------------------


OnLine Upgrade
============================================


OnLine Upgrade with ssh
----------------------------------------------------


OnLine Upgrade with SD Disk
----------------------------------------------------


OnLine Upgrade with USB Disk
----------------------------------------------------