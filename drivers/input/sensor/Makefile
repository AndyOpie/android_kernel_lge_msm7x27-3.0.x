#
# Makefile for the sensor drivers.
#

# Each configuration option enables a list of files.

ifeq ($(CONFIG_MACH_MSM7X27_PECAN),y)
 obj-$(CONFIG_SENSOR_GP2AP)	+= gp2ap002_pecan.o
else
 ifeq ($(CONFIG_MACH_MSM7X27_THUNDERG),y)
  obj-$(CONFIG_SENSOR_GP2AP)	+= gp2ap002_thunderg.o
 else
  ifeq ($(CONFIG_MACH_MSM7X27_THUNDERC),y)
   obj-$(CONFIG_SENSOR_GP2AP)	+= gp2ap002_thunderc.o
  else
   obj-$(CONFIG_SENSOR_GP2AP)	+= gp2ap002.o
  endif
 endif
endif

obj-$(CONFIG_SENSOR_BMA150)	+= bma150.o
obj-$(CONFIG_SENSOR_BMA250) += bma250_driver.o
ifeq ($(CONFIG_MACH_MSM7X27_ALESSI), y)
obj-$(CONFIG_SENSOR_KR3DM)	+= kr3dm_alessi.o
else
ifeq ($(CONFIG_MACH_MSM7X27_PECAN), y)
obj-$(CONFIG_SENSOR_KR3DM)	+= kr3dm_pecan.o
else
obj-$(CONFIG_SENSOR_KR3DM)	+= kr3dm.o
endif
endif
ifeq ($(CONFIG_MACH_MSM7X27_PECAN), y)
obj-$(CONFIG_SENSOR_KR3DH)	+= kr3dh_pecan.o
else
obj-$(CONFIG_SENSOR_KR3DH)	+= kr3dh.o
endif
obj-$(CONFIG_SENSOR_AK8973)	+= akm8973.o
obj-$(CONFIG_SENSOR_AMI602) += ami602.o
ifeq ($(CONFIG_MACH_MSM7X27_ALESSI), y)
obj-$(CONFIG_SENSOR_AMI304) += ami304_alessi.o
else
ifeq ($(CONFIG_MACH_MSM7X27_PECAN), y)
obj-$(CONFIG_SENSOR_AMI304) += ami304_pecan.o
else
obj-$(CONFIG_SENSOR_AMI304) += ami304.o
endif
endif
obj-$(CONFIG_SENSOR_APDS9190) += apds9190.o
obj-$(CONFIG_SENSORS_APDS9801) += apds9801.o

