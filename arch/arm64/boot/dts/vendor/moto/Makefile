ifeq ($(CONFIG_BUILD_ARM64_DT_OVERLAY),y)
    ifeq ($(CONFIG_RACER_DTB),y)
        dtbo-$(CONFIG_RACER_DTB) += \
                racer/lito-racer_01.dtbo \
                racer/lito-racer_02.dtbo \
                racer/lito-racer_03.dtbo
	endif
    ifeq ($(CONFIG_KIEV_DTB),y)
        dtbo-$(CONFIG_KIEV_DTB) += \
                kiev/lagoon-kiev_01.dtbo \
                kiev/lagoon-kiev_02.dtbo
    endif
endif

always		:= $(dtb-y) $(dtbo-y)
subdir-y	:= $(dts-dirs)
clean-files    := *.dtb *.dtbo
