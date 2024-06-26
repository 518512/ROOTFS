# 简介
- 小白一枚，根据各路大神教程，编译自用PVE CT / LXC 模板，Arm&x86_x64版 ROOTFS。
- 基于 [Zane-E/ROOTFS](https://github.com/Zane-E/ROOTFS) 、[217heidai/OpenWrt-Builder](https://github.com/217heidai/OpenWrt-Builder)的缝合产物。
- 为什么要有两个版本的OpenWRT？
- 仅限于就自身使用需求来看，ImmortalWrt更适合作为主路由，LEDE更适合旁路网关，或者无IPV6 RA设置需求的。
## LEDE ARM X86_X64
插件：  
- 基础功能  
- IPV6  
- Wireguard  
- SSR Plus+  
- PW  
- PW2  
- OC  
- Argon 主题  
- AdGuard Home  
- modns  
- upnp  
- ZeroTier  
- Turbo ACC  
- ShutDown/关机  
- ......  
- **待解决，直接使用管理界面无法打开，需更改uhttpd注释掉 443 相关的两行。 https://github.com/coolsnowwolf/lede/issues/11546 ！**
## ImmortalWrt X86_X64
- 基础功能  
- IPV6
- USB网卡等
- Wireguard  
- PW  
- OC 
- Argon 主题   
- modns  
- upnp  
- Turbo ACC  
- ShutDown/关机  
- ......  
## 感谢
- [Zane-E/ROOTFS](https://github.com/Zane-E/ROOTFS)
- [https://github.com/haiibo/OpenWrt](https://github.com/haiibo/OpenWrt)
- [https://github.com/xYx-c/build-openwrt](https://github.com/xYx-c/build-openwrt)
- [217heidai/OpenWrt-Builder](https://github.com/217heidai/OpenWrt-Builder)

**English** | [中文](https://p3terx.com/archives/build-openwrt-with-github-actions.html)
# Actions-OpenWrt

[![LICENSE](https://img.shields.io/github/license/mashape/apistatus.svg?style=flat-square&label=LICENSE)](https://github.com/P3TERX/Actions-OpenWrt/blob/master/LICENSE)
![GitHub Stars](https://img.shields.io/github/stars/P3TERX/Actions-OpenWrt.svg?style=flat-square&label=Stars&logo=github)
![GitHub Forks](https://img.shields.io/github/forks/P3TERX/Actions-OpenWrt.svg?style=flat-square&label=Forks&logo=github)

A template for building OpenWrt with GitHub Actions

## Usage

- Click the [Use this template](https://github.com/P3TERX/Actions-OpenWrt/generate) button to create a new repository.
- Generate `.config` files using [Lean's OpenWrt](https://github.com/coolsnowwolf/lede) source code. ( You can change it through environment variables in the workflow file. )
- Push `.config` file to the GitHub repository.
- Select `Build OpenWrt` on the Actions page.
- Click the `Run workflow` button.
- When the build is complete, click the `Artifacts` button in the upper right corner of the Actions page to download the binaries.

## Tips

- It may take a long time to create a `.config` file and build the OpenWrt firmware. Thus, before create repository to build your own firmware, you may check out if others have already built it which meet your needs by simply [search `Actions-Openwrt` in GitHub](https://github.com/search?q=Actions-openwrt).
- Add some meta info of your built firmware (such as firmware architecture and installed packages) to your repository introduction, this will save others' time.

## Credits

- [Microsoft Azure](https://azure.microsoft.com)
- [GitHub Actions](https://github.com/features/actions)
- [OpenWrt](https://github.com/openwrt/openwrt)
- [Lean's OpenWrt](https://github.com/coolsnowwolf/lede)
- [tmate](https://github.com/tmate-io/tmate)
- [mxschmitt/action-tmate](https://github.com/mxschmitt/action-tmate)
- [csexton/debugger-action](https://github.com/csexton/debugger-action)
- [Cowtransfer](https://cowtransfer.com)
- [WeTransfer](https://wetransfer.com/)
- [Mikubill/transfer](https://github.com/Mikubill/transfer)
- [softprops/action-gh-release](https://github.com/softprops/action-gh-release)
- [ActionsRML/delete-workflow-runs](https://github.com/ActionsRML/delete-workflow-runs)
- [dev-drprasad/delete-older-releases](https://github.com/dev-drprasad/delete-older-releases)
- [peter-evans/repository-dispatch](https://github.com/peter-evans/repository-dispatch)
- [softprops/action-gh-release](https://github.com/softprops/action-gh-release)
- [Zane-E/ROOTFS](https://github.com/Zane-E/ROOTFS)
- [https://github.com/haiibo/OpenWrt](https://github.com/haiibo/OpenWrt)
- [https://github.com/xYx-c/build-openwrt](https://github.com/xYx-c/build-openwrt)
## License

[MIT](https://github.com/P3TERX/Actions-OpenWrt/blob/main/LICENSE) © [**P3TERX**](https://p3terx.com)
