# (C) Copyright 2018,Ratta Inc.
#
# SPDX-License-Identifier:	GPL-2.0+
#

obj-y  := ratta_sn100.o

extra-$(CONFIG_USE_PLUGIN) :=  plugin.bin
$(obj)/plugin.bin: $(obj)/plugin.o
	$(OBJCOPY) -O binary --gap-fill 0xff $< $@
