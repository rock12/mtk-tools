Simple... let's say you unpack a boot.img:
unpack-MTK.pl boot.img
This extracts the kernel (it will be named boot.img-kernel.img) and the ramdisk folder (it will be named boot.img-ramdisk).

In order to repack, you should run:
repack-MTK.pl boot.img-kernel.img boot.img-ramdisk new-boot.img
If you are repacking a recovery.img, then it should be:
Code:
repack-MTK.pl -recovery recovery.img-kernel.img recovery.img-ramdisk
