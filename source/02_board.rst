======================
Product Brief 
======================

NetBot is based on MT7620A Soc, designed by MedeaTek for wireless router and iot solution. The specifications as below:

.. table:: Specifications
   :widths: 20 80
   :align: left

   ===========      ===================================
   Soc                 MT7620A@600MHz
   Memory              256MB
   Flash               SPI Flash 16M
   USB                 4xUSB Hub
   Ethernet            1xRJ45
   Wifi                builtin AP
   LED                 7xLed, GPIOs
   Uart                1 Debug Uart
   Power
   RTC                 NXP PCF8563
   ===========      ===================================


Partition Table
=============================

The SPI Flash Disk is splited into different partitions based on the basic openWRT Flash Layout:

.. table:: Partitions
   :widths: 20 20 60
   :align: left

   ===========      ================     ============================================================================
   partition             size              description
   ===========      ================     ============================================================================
   u-boot                                   boot loader binary, first loaded and prepare for loading kernel.   
   u-boot-env                               boot loader env, upgrade cmds, tftp paras.
   factory                                  factory configs, aka wifi tuning paras.    
   firmware                                 firmware binary, contains kernel & rootfs.                        
   kernel                                   linux kernel, belongs to firmware.                           
   rootfs                                   basic rootfs, read only, belongs to firmware.             
   rootfs_data                              user data, could be customized.
   ===========      ================     ============================================================================