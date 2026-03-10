<div align="center">
<a href="https://github.com/matheusc457/MPatch/releases/latest"><img src="https://images.weserv.nl/?url=https://raw.githubusercontent.com/bmax121/APatch/main/app/src/main/ic_launcher-playstore.png&mask=circle" style="width: 128px;" alt="logo"></a>

<h1 align="center">MPatch</h1>

[![Latest Release](https://img.shields.io/github/v/release/matheusc457/MPatch?label=Release&logo=github)](https://github.com/matheusc457/MPatch/releases/latest)
[![GitHub License](https://img.shields.io/github/license/matheusc457/MPatch?logo=gnu)](/LICENSE)

</div>

The patching of Android kernel and Android system, now with ARMv7 support.

- A fork of [APatch](https://github.com/bmax121/APatch) focused on bringing support to **ARMv7 (armeabi-v7a)** devices.
- APM: Support for modules similar to Magisk.
- KPM: Support for modules that allow you to inject any code into the kernel (Provides kernel function `inline-hook` and `syscall-table-hook`).
- MPatch relies on [KernelPatch](https://github.com/bmax121/KernelPatch/).
- The MPatch UI and the APModule source code have been derived and modified from [KernelSU](https://github.com/tiann/KernelSU).

Or download the latest APK from the [Releases Section](https://github.com/matheusc457/MPatch/releases/latest).

## Supported Versions

- Supports **ARM64** and **ARMv7 (armeabi-v7a)** architectures.
- Only supports Android kernel versions 3.18 - 6.12

> ARMv7 support is currently under active development. Contributions are welcome!

Support for Samsung devices with security protection: Planned

## Requirement

Kernel configs:

- `CONFIG_KALLSYMS=y` and `CONFIG_KALLSYMS_ALL=y`

- `CONFIG_KALLSYMS=y` and `CONFIG_KALLSYMS_ALL=n`: Initial support

## Security Alert

The **SuperKey** has higher privileges than root access.  
Weak or compromised keys can lead to unauthorized control of your device.  
It is critical to use robust keys and safeguard them from exposure to maintain the security of your device.

## Roadmap

- [x] Fork APatch
- [ ] Add `armeabi-v7a` ABI to manager native builds
- [ ] Port kpatch stubs to Thumb-2/ARM32
- [ ] Full ARMv7 kernel patching support
- [ ] Testing on ARMv7 devices

## Get Help

### Usage

For usage, please refer to [APatch's official documentation](https://apatch.dev) as a reference.  
MPatch-specific documentation is coming soon.

## Credits

- [APatch](https://github.com/bmax121/APatch): The upstream project this fork is based on.
- [KernelPatch](https://github.com/bmax121/KernelPatch/): The core.
- [Magisk](https://github.com/topjohnwu/Magisk): magiskpolicy.
- [KernelSU](https://github.com/tiann/KernelSU): App UI, and Magisk module like support.

## License

MPatch is licensed under the GNU General Public License v3 [GPL-3](http://www.gnu.org/copyleft/gpl.html).

