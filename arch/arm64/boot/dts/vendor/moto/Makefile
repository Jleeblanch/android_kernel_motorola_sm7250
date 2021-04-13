ifeq ($(CONFIG_MMI_DEVICE_DTBS),y)
ifneq ($(CONFIG_BUILD_ARM64_DT_OVERLAY),y)
$(error Moto DT w/o overlay is undefined!!!)
endif
ifeq ($(CONFIG_RACER_DTB),y)
dtbo-$(CONFIG_RACER_DTB) += \
                racer/lito-racer_01.dtbo \
                racer/lito-racer_02.dtbo \
                racer/lito-racer_03.dtbo
endif

ifeq ($(CONFIG_KIEV_DTB),y)
include $(srctree)/arch/arm64/boot/dts/vendor/moto/kiev/Makefile
endif
endif

always		:= $(dtb-y) $(dtbo-y)
subdir-y	:= $(dts-dirs)
clean-files    := *.dtb *.dtbo
