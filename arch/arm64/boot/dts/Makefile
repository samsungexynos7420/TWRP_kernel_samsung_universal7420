dtb-$(CONFIG_BOARD_ZEROFLTE) += exynos7420-zeroflte_eur_open_00.dtb \
	exynos7420-zeroflte_eur_open_01.dtb \
	exynos7420-zeroflte_eur_open_02.dtb \
	exynos7420-zeroflte_eur_open_03.dtb \
	exynos7420-zeroflte_eur_open_04.dtb \
	exynos7420-zeroflte_eur_open_05.dtb \
	exynos7420-zeroflte_eur_open_06.dtb \
	exynos7420-zeroflte_eur_open_07.dtb

dtb-$(CONFIG_BOARD_ZEROLTE) += exynos7420-zerolte_eur_open_01.dtb \
	exynos7420-zerolte_eur_open_02.dtb \
	exynos7420-zerolte_eur_open_03.dtb \
	exynos7420-zerolte_eur_open_04.dtb \
	exynos7420-zerolte_eur_open_05.dtb \
	exynos7420-zerolte_eur_open_06.dtb \
	exynos7420-zerolte_eur_open_07.dtb \
	exynos7420-zerolte_eur_open_08.dtb

dtb-$(CONFIG_BOARD_ZENLTE) += exynos7420-zenlte_eur_open_00.dtb \
	exynos7420-zenlte_eur_open_09.dtb
	
dtb-$(CONFIG_BOARD_NOBLELTE) += exynos7420-noblelte_eur_open_00.dtb \
	exynos7420-noblelte_eur_open_09.dtb

targets += dtbs

DTB_NAMES := $(subst $\",,$(CONFIG_BUILD_ARM64_APPENDED_DTB_IMAGE_NAMES))
ifneq ($(DTB_NAMES),)
DTB_LIST := $(addsuffix .dtb,$(DTB_NAMES))
else
DTB_LIST := $(dtb-y)
endif
targets += $(DTB_LIST)

dtbs: $(addprefix $(obj)/, $(DTB_LIST))

clean-files := dts/*.dtb *.dtb
