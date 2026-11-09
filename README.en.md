# TCL S8 Screen Tuner 1.0

| [简体中文](README.zh-CN.md) | **English** |
|:---:|:---:|

TCL S8 Screen Tuner is an Android display adjustment utility for the TCL NXTPAPER S8. It uses the device's MediaTek PQ and Android display interfaces to adjust image parameters, with controls available from both the main screen and a floating panel.

## Features

- Adjust contrast, saturation, Gamma, picture brightness, sharpness, blue-light strength, and RGB gains.
- Adjust the Gamma LUT curve from 0% to 200%. At 100%, the app restores the factory curve for the current Gamma index. The curve interface does not provide hardware readback.
- Toggle Color Effect, Dynamic Contrast, and Android color inversion.
- Preview and adjust PQ parameters in a floating panel over other apps. Parameter values stay synchronized between the main screen and the panel.
- Apply the recommended preset or restore the device's PQ defaults from either interface.
- Tap a displayed value to enter an absolute value.

## Requirements

- Root access is required. Grant superuser access to `com.codex.s8tuner` in your root manager.
- Grant the app permission to display over other apps to use the floating panel.
- This build was primarily verified on the TCL NXTPAPER S8 `9288A_EEA / Da_Vinci_4G` firmware. Other devices and firmware versions are untested.
- Chameleon controls depend on the device driver. The current S8 driver may reject writes requesting a nonzero strength; the app follows the state supported by the device.

## Safety Notice

This app uses root privileges to access display control interfaces. Available controls and their effects depend on the device, Android version, and display driver; unsupported writes may be rejected. Root operations and display adjustments can affect device operation or image quality. Use the app at your own risk. The software is provided as is, without warranty.

## GitHub Release

- Version: `1.0` (version code `1`)
- APK: `S8-screen-tuner-1.0.apk`
- SHA-256: `ABD98603464F5DD924030D478612E066E6A5756481E47190DAB63F1856709AA8`

## What's New

- Initial TCL S8 release with MediaTek PQ controls, Gamma LUT, RGB gains, toggle controls, and a floating panel.
- Added a recommended preset, factory-default reset, and synchronized values between the main screen and floating panel.
