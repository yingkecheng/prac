KERNELDIR := /home/yingkecheng/Projects/LinuxDriverStudy/my_linux/
CURRENT_PATH := $(shell pwd)
ENV	:= ARCH=arm CROSS_COMPILE=/home/yingkecheng/Applications/Compilers/gcc-linaro-4.9.4-2017.01-x86_64_arm-linux-gnueabihf/bin/arm-linux-gnueabihf-
obj-m := completion_prac.o

build: kernel_modules

kernel_modules:
	$(MAKE) $(ENV) -C $(KERNELDIR) M=$(CURRENT_PATH) modules

clean:
	$(MAKE) $(ENV) -C $(KERNELDIR) M=$(CURRENT_PATH) clean
