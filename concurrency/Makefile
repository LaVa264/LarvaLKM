obj-m += percpu.o
obj-m += mutex.o
obj-m += spinlocks.o
obj-m += rwlock.o
obj-m += atomic.o
obj-m += completions.o

PWD := $(CURDIR)

all:
	make -C /lib/modules/$(shell uname -r)/build M=$(PWD) modules
clean:
	make -C /lib/modules/$(shell uname -r)/build M=$(PWD) clean