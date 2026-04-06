# STM32MP25 OpenSTLinux Project

## Overview
This project is based on:
- Yocto Project (scarthgap)
- ST OpenSTLinux BSP

## Branch
- scarthgap (latest updates)

## Release Information
- Ecosystem: STM32MPU-Ecosystem v6.2.0
- OpenSTLinux: openstlinux-6.6-yocto-scarthgap-mpu-v26.02.18

## Manifest
This repository provides the repo manifest for OpenSTLinux.

## Quick Start
``` DISTRO=openstlinux-weston MACHINE=stm32mp25-disco source layers/meta-st/scripts/envsetup.sh ```

``` bitbake st-image-waton ```

## Custom Layer
meta-breakout:
https://github.com/Huai0429/meta-breakout

Description:
- Board bring-up
- Device Tree
- Drivers
- Applications

## Documentation
- STM32 MPU Wiki:
https://wiki.st.com/stm32mpu/wiki/STM32MPU_Distribution_Package