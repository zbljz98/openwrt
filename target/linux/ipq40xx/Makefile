include $(TOPDIR)/rules.mk

ARCH:=arm
BOARD:=ipq40xx
BOARDNAME:=Qualcomm Atheros IPQ40XX
FEATURES:=squashfs fpu ramdisk nand
CPU_TYPE:=cortex-a7
CPU_SUBTYPE:=neon-vfpv4
SUBTARGETS:=generic mikrotik

KERNEL_PATCHVER:=5.10
KERNEL_TESTING_PATCHVER:=5.10

KERNELNAME:=zImage Image dtbs

include $(INCLUDE_DIR)/target.mk
DEFAULT_PACKAGES += \
	kmod-usb-dwc3-qcom \
	kmod-leds-gpio kmod-gpio-button-hotplug swconfig \
	kmod-ath10k-ct wpad-basic-wolfssl \
	kmod-usb3 kmod-usb-dwc3 ath10k-firmware-qca4019-ct \
	ath10k-board-qca4019 uboot-envtools autocore-arm

$(eval $(call BuildTarget))
