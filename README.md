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
``` repo init -u git@github.com:Huai0429/stm32mp25-manifest.git -b scarthgap```

```repo sync```

``` DISTRO=openstlinux-weston MACHINE=stm32mp2 source layers/meta-st/scripts/envsetup.sh ```

``` bitbake-layers add-layer ../layers/meta-sdbus-lite```


``` bitbake st-image-weston ```

## Custom Layer
### meta-sdbus-lite
https://github.com/Huai0429/meta-sdbus-lite

The **sdbus-lite** library based on sdbus to help you simplify the dbus code complexity.\
A streamlined C library that wraps libsystemd sd-bus to simplify D-Bus IPC. \
It provides easy-to-use APIs for initialization, method invocation, signal handling, and property management, enabling unified and reusable IPC across multiple applications.

### meta-breakout
https://github.com/Huai0429/meta-breakout

Description:
- Board bring-up
- Device Tree
- Drivers
- Applications


## Documentation
- STM32 MPU Wiki:
https://wiki.st.com/stm32mpu/wiki/STM32MPU_Distribution_Package