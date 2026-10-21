VERSION=0.0.1
obj-m+=panda.o

link:
	sudo dkms add `pwd`

build:
	sudo dkms build panda/$(VERSION) --force

install:
	sudo dkms install panda/$(VERSION) --force

all:	build install

uninstall:
	sudo dkms uninstall panda/$(VERSION)
	sudo dkms remove panda/$(VERSION) --all

