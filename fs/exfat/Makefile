obj-m += exfat.o
exfat-y	:= exfat_core.o exfat_super.o exfat_api.o exfat_blkdev.o exfat_cache.o \
		exfat_data.o exfat_bitmap.o exfat_nls.o exfat_oal.o exfat_upcase.o

all:
	make -C /lib/modules/$(shell uname -r)/build M=$(PWD) modules
 
clean:
	make -C /lib/modules/$(shell uname -r)/build M=$(PWD) clean
