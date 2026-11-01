<div align="center">

# <img src="https://raw.githubusercontent.com/rubygsi/rubyGSI/main/assets/icon.png" width="120" alt="rubyGSI Logo" />

# 🍎 rubyGSI

**A curated collection of custom GSI (Generic System Images) built from various stock firmwares.**

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
[![Platform](https://img.shields.io/badge/Platform-Android%2013%2B-brightgreen.svg)]()
[![Architecture](https://img.shields.io/badge/Architecture-arm64--ab-orange.svg)]()
[![Status](https://img.shields.io/badge/Status-Experimental-red.svg)]()

[![GitHub Stars](https://img.shields.io/github/stars/rubygsi/rubyGSI?style=social)]()
[![GitHub Forks](https://img.shields.io/github/forks/rubygsi/rubyGSI?style=social)]()
[![GitHub Issues](https://img.shields.io/github/issues/rubygsi/rubyGSI)]()

<br>

**[English](#english) | [中文](#chinese)**

</div>

---

## ⚠️ DISCLAIMER / 免责声明

> **⚠️ READ BEFORE FLASHING / 刷机前必读**
> 
> This project is **EXPERIMENTAL**. These images are built for personal testing and may contain bugs, bootloops, or hardware incompatibilities. The author is **NOT responsible** for bricked devices, voided warranties, or data loss. **Always back up your data** and ensure you have a way to restore your device (e.g., SP Flash Tool, Fastboot ROM) before proceeding.
>
> 本项目为**实验性**项目。这些镜像仅供个人测试使用，可能存在Bug、无法开机或硬件不兼容等问题。作者**不对**设备变砖、保修失效或数据丢失负责。**刷机前请务必备份数据**，并确保您有恢复设备的方法（如SP Flash Tool、Fastboot ROM）。

---

<a name="english"></a>
# 🇬🇧 English

## 📖 About rubyGSI

**rubyGSI** is a repository dedicated to providing **custom GSI (Generic System Images)** built from various stock firmwares. Our goal is to offer a unified place to download pre-built GSI images that work on a wide range of Android devices with Project Treble support (arm64).

We do not focus on a single brand or OS. Instead, we collect and build images from multiple sources, making it easier for users to find a GSI that suits their needs. Whether you're testing a new UI, developing, or just exploring, rubyGSI aims to be your hub.

## 🧐 What is a GSI?

A **GSI (Generic System Image)** is a universal Android system image that can be flashed onto any device that supports **Project Treble**. It allows you to run a different version of Android (or a custom ROM) without needing a device-specific build. 

Our GSIs are built using [MysticGSI](https://github.com/MysticGSI/mysticgsi), a powerful tool that converts stock firmware into a GSI-compatible image.

## 📦 Available Releases

You can find all available GSI images in the **[Releases](https://github.com/rubygsi/rubyGSI/releases)** section.

| Image Name | Source Firmware | Android Version | Status |
| :--- | :--- | :--- | :--- |
| `rubyGSI-xyz-arm64.img` | *(Various)* | Android 14/15/16 | 🧪 Testing |
| `rubyGSI-abc-arm64.img` | *(Various)* | Android 14/15/16 | ✅ Stable |
| *(More coming soon)* | *(More coming soon)* | *(More coming soon)* | *(More coming soon)* |

> **Note:** Image names and sources are intentionally generic. We do not list specific brand names to keep the focus on the GSI itself.

## 🛠️ How to Install

We recommend using **DSU Sideloader** for a safe, non-destructive installation. This method boots the GSI as a "guest" system without touching your primary Android installation.

### Method 1: DSU Sideloader (Recommended)
1. Download the `.img` file from the **[Releases](https://github.com/rubygsi/rubyGSI/releases)** section.
2. Install [DSU Sideloader](https://github.com/VegaBobo/DSU-Sideloader) on your device (requires Root or Shizuku).
3. Open DSU Sideloader, select the downloaded `.img` file, and tap **Install**.
4. Wait for the process to complete. When prompted, **Restart** your device to boot into the GSI.
5. To return to your original system, simply reboot your device and select the "Boot to System" option in the DSU notification.

### Method 2: Custom Recovery (Advanced)
1. Boot into a custom recovery like **Pitch Black Recovery (PBRP)** or **TWRP**.
2. Perform a **Format Data** (type `yes` to confirm).
3. Go to **Install -> Install Image**, select the `.img` file, and choose the **System** partition.
4. Flash the image and reboot.

## 🧪 Known Issues

Because GSIs are generic and not optimized for specific hardware, you may encounter the following issues:
- **Camera**: May not work or may crash (proprietary drivers missing).
- **Sound**: Microphone or speaker issues are common.
- **Fingerprint**: Biometric scanners often fail to initialize.
- **Battery**: Higher battery drain due to lack of vendor optimizations.
- **VoLTE**: May not work on some carriers.

## 🤝 Contributing

We welcome contributions! If you have a working GSI build you'd like to share, or if you've found a fix for a specific device, please open an **Issue** or submit a **Pull Request**.

## 📜 License

This project is licensed under the **GNU General Public License v3.0**. See the [LICENSE](LICENSE) file for details.

---

<a name="chinese"></a>
# 🇨🇳 中文

## 📖 关于 rubyGSI

**rubyGSI** 是一个专注于提供**自定义 GSI（通用系统镜像）**的代码仓库。我们的目标是为支持 Project Treble（arm64）的 Android 设备提供一个统一的 GSI 镜像下载平台。

我们不专注于单一品牌或操作系统。相反，我们收集并构建来自多个来源的镜像，帮助用户更轻松地找到适合自己的 GSI。无论您是测试新 UI、进行开发，还是仅仅出于好奇，rubyGSI 都致力于成为您的中心。

## 🧐 什么是 GSI？

**GSI（通用系统镜像）** 是一种通用的 Android 系统镜像，可以刷入任何支持 **Project Treble** 的设备。它允许您运行不同版本的 Android（或自定义 ROM），而无需设备专用的构建版本。

我们的 GSI 使用 [MysticGSI](https://github.com/MysticGSI/mysticgsi) 构建，这是一个将官方固件转换为 GSI 兼容镜像的强大工具。

## 📦 可用版本

您可以在 **[Releases](https://github.com/rubygsi/rubyGSI/releases)** 部分找到所有可用的 GSI 镜像。

| 镜像名称 | 来源固件 | Android 版本 | 状态 |
| :--- | :--- | :--- | :--- |
| `rubyGSI-xyz-arm64.img` | *(多种)* | Android 14/15/16 | 🧪 测试中 |
| `rubyGSI-abc-arm64.img` | *(多种)* | Android 14/15/16 | ✅ 稳定 |
| *(更多即将推出)* | *(更多即将推出)* | *(更多即将推出)* | *(更多即将推出)* |

> **注意**：镜像名称和来源有意保持通用。我们不会列出具体品牌名称，以保持对 GSI 本身的关注。

## 🛠️ 如何安装

我们推荐使用 **DSU Sideloader** 进行安全、无损的安装。此方法将 GSI 作为“访客”系统启动，不会影响您的主要 Android 系统。

### 方法一：DSU Sideloader（推荐）
1. 从 **[Releases](https://github.com/rubygsi/rubyGSI/releases)** 部分下载 `.img` 文件。
2. 在您的设备上安装 [DSU Sideloader](https://github.com/VegaBobo/DSU-Sideloader)（需要 Root 或 Shizuku）。
3. 打开 DSU Sideloader，选择下载的 `.img` 文件，然后点击 **Install**。
4. 等待进程完成。当系统提示时，**重启**设备以启动 GSI。
5. 要返回原始系统，只需重启设备，并在 DSU 通知中选择“Boot to System”选项。

### 方法二：自定义 Recovery（高级）
1. 启动进入自定义 Recovery，如 **Pitch Black Recovery (PBRP)** 或 **TWRP**。
2. 执行 **Format Data**（输入 `yes` 确认）。
3. 转到 **Install -> Install Image**，选择 `.img` 文件，并选择 **System** 分区。
4. 刷入镜像并重启。

## 🧪 已知问题

由于 GSI 是通用的，并未针对特定硬件进行优化，您可能会遇到以下问题：
- **相机**：可能无法工作或崩溃（缺少专有驱动）。
- **声音**：麦克风或扬声器问题很常见。
- **指纹**：生物识别扫描器通常无法初始化。
- **电池**：由于缺少厂商优化，电池消耗较高。
- **VoLTE**：在某些运营商上可能无法使用。

## 🤝 贡献

我们欢迎贡献！如果您有可用的 GSI 构建版本想要分享，或者您找到了针对特定设备的修复方法，请打开 **Issue** 或提交 **Pull Request**。

## 📜 许可证

本项目根据 **GNU 通用公共许可证 v3.0** 授权。详情请参阅 [LICENSE](LICENSE) 文件。

---

<div align="center">
  
**Made with ❤️ by the rubyGSI Community.**

**由 rubyGSI 社区用 ❤️ 制作。**

</div>
