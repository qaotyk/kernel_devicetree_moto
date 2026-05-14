#Only include Motorola DTBs
ifeq ($(CONFIG_MMI_DEVICE_DTBS),y)
ifneq ($(CONFIG_BUILD_ARM64_DT_OVERLAY),y)
	$(error Motorola DT w/o overlay is undefined)
endif

# Add 1k of padding to the DTBs to allow for environment variables
# to be runtime added by the bootloader (i.e. /chosen properties)
DTC_FLAGS += -p 1024

# sm6150-common devices

# CONFIG_DOHA_DTB (Moto G8 Plus)
dtbo-$(CONFIG_DOHA_DTB) += \
	trinket-doha-evt1-overlay.dtbo \
	trinket-doha-evt2-overlay.dtbo \
	trinket-doha-dvt2-overlay.dtbo

trinket-doha-evt1-overlay.dtbo-base :=  trinket-doha-base.dtb
trinket-doha-evt2-overlay.dtbo-base :=  trinket-doha-base.dtb
trinket-doha-dvt2-overlay.dtbo-base :=  trinket-doha-base.dtb

# CONFIG_ROMA_DTB (Moto Tab P11)
dtbo-$(CONFIG_ROMA_DTB) += \
	trinket-roma-evb-overlay.dtbo \
	trinket-roma-evt1-overlay.dtbo \
	trinket-roma-evt2-overlay.dtbo

trinket-roma-evb-overlay.dtbo-base :=  trinket-roma-base.dtb
trinket-roma-evt1-overlay.dtbo-base :=  trinket-roma-base.dtb
trinket-roma-evt2-overlay.dtbo-base :=  trinket-roma-base.dtb

# CONFIG_RAV_DTB (Moto G8, G Fast)
dtbo-$(CONFIG_RAV_DTB) += \
	trinket-rav-evb1-overlay.dtbo \
	trinket-rav-evb1-na-overlay.dtbo \
	trinket-rav-evb2-overlay.dtbo \
	trinket-rav-evb2-na-overlay.dtbo \
	trinket-rav-pvt1-overlay.dtbo \
	trinket-rav-pvt1-na-overlay.dtbo

trinket-rav-evb1-overlay.dtbo-base :=  trinket-rav-base.dtb
trinket-rav-evb1-na-overlay.dtbo-base :=  trinket-rav-base.dtb
trinket-rav-evb2-overlay.dtbo-base :=  trinket-rav-base.dtb
trinket-rav-evb2-na-overlay.dtbo-base :=  trinket-rav-base.dtb
trinket-rav-pvt1-overlay.dtbo-base :=  trinket-rav-base.dtb
trinket-rav-pvt1-na-overlay.dtbo-base :=  trinket-rav-base.dtb

# CONFIG_SOFIA_DTB (Moto G Power EEUU)
dtbo-$(CONFIG_SOFIA_DTB) += \
	trinket-sofia-evb1-overlay.dtbo \
	trinket-sofia-evt-overlay.dtbo \
	trinket-sofia-dvt1a-overlay.dtbo \
	trinket-sofia-dvt1b-overlay.dtbo \
	trinket-sofia-dvt2-overlay.dtbo \
	trinket-sofia-pvt-overlay.dtbo

trinket-sofia-evb1-overlay.dtbo-base :=  trinket-sofia-base.dtb
trinket-sofia-evt-overlay.dtbo-base :=  trinket-sofia-base.dtb
trinket-sofia-dvt1a-overlay.dtbo-base :=  trinket-sofia-base.dtb
trinket-sofia-dvt1b-overlay.dtbo-base :=  trinket-sofia-base.dtb
trinket-sofia-dvt2-overlay.dtbo-base :=  trinket-sofia-base.dtb
trinket-sofia-pvt-overlay.dtbo-base :=  trinket-sofia-base.dtb
