# Z490-UD-rev-1.0 running on OpenCore 0.6.9 (Catalina)
## System Specs

- MB: Gigabyte Z490 UD Rev 1.0
- CPU: Intel i7 10700
- GPU: Radeon RX 580

## BIOS Settings

- Bios Version: F20

### BIOS Features

**Disabled**

- Fast Boot
- Secure Boot
- VT-d
- SuperIO
  - Serial Port [ fixes stuttering ]
- Legacy USB Support

**Enabled**

- 4G Decoding
  - Re-size BAR support: Auto
- Hyper-threading
- CSM Support [*my system won't properly boot without this on due to the GPU*]
  - Windows 10 Features: Other
  - Storage Boot Option Control - UEFI

## What's Working

- [x] Installation
- [x] Booting
- [x] GPU
- [x] Bootcamp
- [x] Sleep
- [x] External Audio (USB Audio Card)
- [x] USB
- [ ] MB Audio
- [ ] iGPU

*My setup does not use iGPU or MB Audio therefore these features have not been implemented n'or tested. Feel free to open an issue or make a PR to add support for these!*

## How can I use this ?

You can just use the EFI folder in the repository as is to boot either a Catalina installation disk or boot into your existing Mac installation.

Do test using an USB stick before overwriting any existing Clover/OpenCore installation as issues could occur.

If you find a better configuration for these specs, feel free to make a pull request or open an issue!

## FAQ

### My computer does not seem to boot

Without CSM Support enabled (and 4G Decoding), the setup does not boot with my Sapphire Radeon 580 GPU for some reason.

## Special Thanks To

- Apple for MacOS
- The OpenCore team
- The Hackintosh Reddit Community
- InsanelyMac for a ton of helpful resources
- The InsanelyHack Discord community for help and support
- [The OpenCore Vanilla Desktop Guide](https://khronokernel-2.gitbook.io/opencore-vanilla-desktop-guide/)
- [USBToolBox Tool](https://github.com/USBToolBox/tool)

