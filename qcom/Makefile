#Only include Motorola DTBs
ifeq ($(CONFIG_MMI_DEVICE_DTBS),y)
ifneq ($(CONFIG_BUILD_ARM64_DT_OVERLAY),y)
	$(error Motorola DT w/o overlay is undefined)
endif

# Add 1k of padding to the DTBs to allow for environment variables
# to be runtime added by the bootloader (i.e. /chosen properties)
DTC_FLAGS += -p 1024

# sm6150-common devices

# CONFIG_DOHA_DTB
dtbo-$(CONFIG_DOHA_DTB) += \
	trinket-doha-evt1-overlay.dtbo \
	trinket-doha-evt2-overlay.dtbo \
	trinket-doha-dvt2-overlay.dtbo

trinket-doha-evt1-overlay.dtbo-base :=  trinket-doha-base.dtb
trinket-doha-evt2-overlay.dtbo-base :=  trinket-doha-base.dtb
trinket-doha-dvt2-overlay.dtbo-base :=  trinket-doha-base.dtb