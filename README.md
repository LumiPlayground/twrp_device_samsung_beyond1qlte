# TWRP Device Tree for Samsung Galaxy S10 (Snapdragon)

## Notes

FBEv1 decryption might or might not work and only if no password was set

## Kernel Source

Prebuilt from latest Android 12 firmware (SCV41KDU1DWC1)

## How to build

This device tree was tested and is fully compatible with [minimal-manifest-twrp](https://github.com/minimal-manifest-twrp/platform_manifest_twrp_aosp).

1. Set up the build environment following the instructions [here](https://github.com/minimal-manifest-twrp/platform_manifest_twrp_aosp/blob/twrp-12.1/README.md#getting-started)

2. In the root folder of the fetched repo, clone the device tree:

```bash
git clone https://github.com/LumiPlayground/twrp_device_samsung_beyond1qlte.git -b android-12.1 device/samsung/beyond1qlte
```

3. To build:

```bash
export ALLOW_MISSING_DEPENDENCIES=true
. build/envsetup.sh
lunch twrp_beyond1qlte-eng
mka recoveryimage
```
