
include $(srctree)/drivers/misc/mediatek/Makefile.custom

# Module project related part

ifeq ($(CONFIG_MTK_SENSOR_SUPPORT),y)
ifeq ($(CONFIG_MTK_AP3220),y)
obj-y	+=  alsps/ap3220/
endif

ifeq ($(CONFIG_MTK_BMA222E_AUTO),y)
obj-y	+=  accelerometer/bma222E_auto/
endif

ifeq ($(CONFIG_MTK_KXTJ2_1009_AUTO),y)
obj-y	+=  accelerometer/KXTJ2_1009_auto/
endif

ifeq ($(CONFIG_MTK_AKM09911),y)
obj-y	+=  magnetometer/akm09911/
endif

ifeq ($(CONFIG_MTK_L3GD20),y)
obj-y   +=  gyroscope/l3gd20/
endif

ifeq ($(CCONFIG_MTK_BMI058_AUTO),y)
obj-y   +=  gyroscope/bmi058/
endif

ifeq ($(CONFIG_MTK_BMG160),y)
obj-y   +=  gyroscope/bmg160/
endif
endif

ifneq ($(CONFIG_ARCH_MTK_PROJECT),)
ARCH_MTK_PROJECT := $(shell echo $(CONFIG_ARCH_MTK_PROJECT))
obj-y	+= core/
obj-y	+= dct/dct/
endif

#obj-y	+=  hdmi/
obj-y	+=  flashlight/
obj-y	+=  camera/camera/
obj-y	+=  vibrator/
obj-y	+=  leds/
obj-y	+=  keypad/
obj-y	+=  sound/
obj-y	+=  accdet/
obj-y	+=  partition/
