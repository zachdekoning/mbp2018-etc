obj-m += applesmc_t2_kmod.o

MY_CFLAGS += -g -DDEBUG
ccflags-y += ${MY_CFLAGS}
CC += ${MY_CFLAGS}
KERNEL_VERSION := $(shell uname -r)

all:
        make -C /lib/modules/$(KERNEL_VERSION)/build M=$(PWD) modules

clean:
        make -C /lib/modules/$(KERNEL_VERSION)/build M=$(PWD) clean
