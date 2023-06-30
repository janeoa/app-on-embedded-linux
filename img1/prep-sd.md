# Preparing the SD card
## as a mac user
* Make sure you are using the correct SD card (note the device number, ex /dev/disk6)
`diskutil list`
* Partition the DISK as MBR with 2 partitions (Default GPT will spawn EFI as first partition)
`diskutil partitionDisk /dev/disk6 2 MBR "MS-DOS FAT32" "P1" 490M "MS-DOS FAT32" "P2" R`
* Copy the image to the SD card
`sudo dd if=/Users/assetmalik/Desktop/untitled\ folder\ 2/Image  of=/dev/disk6 bs=1k seek=33 conv=fsync`
* Format the first partition to VFAT
`sudo diskutil eraseVolume "MS-DOS FAT32" "NEWVOL" /dev/disk6s1`

## OKMX8MM state on the steps
* when the SD card is freshly fully formatted it says `��������`
* when using the flash_sd_bootloader.bin, the system is up, the u-boot is present
* when eraseVolume the first partition, the system is up, the u-boot is failed to load, "Synch Abort" error leads to reset