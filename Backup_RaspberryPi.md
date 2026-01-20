# step 1: Find the SD card device name
``lsblk``
# Unmount the SD card (important!)
``sudo umount /dev/sdb*``
Replace sdb with your actual device name
# Create the backup image
``sudo dd if=/dev/sdb of=/home/username/raspi_backup.img bs=4M status=progress
``
# wait till it finished and you get your image.
