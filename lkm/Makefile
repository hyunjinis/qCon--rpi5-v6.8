CONFIG_MODULE_SIG=n
KERNEL_DIR=/lib/modules/6.8.12-v8-16k+/build
obj-m = vif.o

KDIR := $(KERNEL_DIR)
PWD := $(shell pwd)

CFLAGS += -I/home/rpi1/hjkim/6.8/linux/net/bridge

all:
	$(MAKE) -C $(KDIR) M=$(PWD) modules

clean:
	@rm -rf *.ko
	@rm -rf *.mod.*
	@rm -rf .*.cmd
	@rm -rf *.o
	@rm -rf *.ko.*
	@rm -rf modules.order
	@rm -rf Module.symvers
	@rm -rf .tmp_versions
