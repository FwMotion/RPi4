Customized Raspberry Pi 4 UEFI Firmware Images
==============================================

[![Build status](https://img.shields.io/github/workflow/status/FwMotion/RPi4/UEFI%20firmware%20-%20EDK2%20build.svg?style=flat-square)](https://github.com/FwMotion/RPi4/actions)
[![Github stats](https://img.shields.io/github/downloads/FwMotion/RPi4/total.svg?style=flat-square)](https://github.com/FwMotion/RPi4/releases)
[![Release](https://img.shields.io/github/release-pre/FwMotion/RPi4?style=flat-square)](https://github.com/FwMotion/RPi4/releases)

# Summary

This repository contains installable builds of the official
[EDK2 Raspberry Pi 4 UEFI firmware](https://github.com/tianocore/edk2-platforms/tree/master/Platform/RaspberryPi/RPi4).

For the original builds without customization, visit [the Pi Firmware Task Force's RPi4 repository](https://github.com/pftf/RPi4). Review that page for installation, usage, and other notices.

# Changes from Upstream Builds

The following changes have been applied to customize the build:

1. Disable RAM Limiter by default
2. Include the PoE HAT and PoE+ HAT devicetree overlays
3. Enable the PoE HAT devicetree overlay by default
4. Changed the UEFI Firmware Vendor string
5. Disable the Raspberry Pi firmware rainbow splash

# License

The firmware (`RPI_EFI.fd`) is licensed under the current EDK2 license, which is
[BSD-2-Clause-Patent](https://github.com/tianocore/edk2/blob/master/License.txt).

The other files from the zip archives are licensed under the terms described in the
[Raspberry Pi boot files README](https://github.com/raspberrypi/firmware/blob/master/README.md).

The binary blobs in the `firmware/` directory are licensed under the Cypress wireless driver
license that is found there.
