#
# Makefile for MMC/SD card drivers
#

obj-$(CONFIG_MMC_BLOCK)		+= mmc_block.o
mmc_block-objs			:= block.o queue.o
obj-$(CONFIG_MMC_TEST)		+= mmc_test.o

obj-$(CONFIG_SDIO_UART)		+= sdio_uart.o

ifeq ($(CONFIG_HUAWEI_KERNEL),y)
	obj-$(CONFIG_HUAWEI_KERNEL) += panic_transfer.o
else
	obj-$(CONFIG_APANIC) += panic_transfer.o
endif
