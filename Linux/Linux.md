#### MAN Page - Online ####
http://man7.org/linux/man-pages/dir_all_alphabetic.html#top

#### Set custom resolution ####
http://ubuntuhandbook.org/index.php/2017/04/custom-screen-resolution-ubuntu-desktop/

#### Configure LVM in Linux (pvcreate, lvcreate, vgcreate) ####
https://linoxide.com/linux-how-to/lvm-configuration-linux/

#### Create and Mount a Partition (DISK) ####
https://www.tecmint.com/add-new-disk-to-an-existing-linux/

#### Increase SSH timeout ####
https://bjornjohansen.no/ssh-timeout

#### Change file format (xfs) ####
https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/7/html/storage_administration_guide/ch-xfs


##### Extend/Decrease LVM Size #####
https://www.tecmint.com/extend-and-reduce-lvms-in-linux/

```bash

vgextend rootvg /dev/sdd6

lvdisplay

vgdisplay

lvextend -l +3051 /dev/rootvg/lv_root

xfs_growfs /dev/rootvg/lv_root

```
