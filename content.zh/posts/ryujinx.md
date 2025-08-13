---
title: "Ryujinx 模拟器安装指南"
date: 2025-08-02T00:14:05+03:00
# bookComments: false
# bookSearchExclude: false
---

## 什么是 Ryujinx？

Ryujinx 是一款开源的 Nintendo Switch 模拟器，目标是在电脑上复现 Switch 的游戏体验。它主要使用 C# 开发，注重准确性与性能，支持 Windows 与 Linux（也在一定程度上支持 macOS），可在不同分辨率与帧率下游玩游戏，且常常能提供比原机更好的输出效果。

官方网站： https://ryujinx.app/

{{% columns %}}
- ### Windows
  支持 Windows 10 与 11。大多数用户需要 x64 版本。

  <img src="/images/windows.png" width="100"/>

  {{<button href="https://update.ryujinx.app/download/query?os=win&arch=x64&rc=stable">}}下载 x64{{</button>}}

- ### macOS
  仅正式支持 Apple Silicon Mac。

  <img src="/images/macos.png" width="100"/>

  {{<button href="https://update.ryujinx.app/download/query?os=mac&arch=arm64&rc=stable">}}下载{{</button>}}

- ### Linux（普通包）

  标准 Linux 可执行文件与依赖的打包（tarball）。

  <img src="/images/linux.png" width="100"/>

  {{<button href="https://update.ryujinx.app/download/query?os=linux&arch=x64&rc=stable">}}下载 x64{{</button>}}

  {{<button href="https://update.ryujinx.app/download/query?os=linux&arch=arm64&rc=stable">}}下载 ARM{{</button>}}

{{% /columns %}}

{{% columns %}}

### Linux（AppImage）
适用于大多数现代 Linux 发行版。

<img src="/images/linux.png" width="100"/>

{{<button href="https://update.ryujinx.app/download/query?os=linuxai&arch=x64&rc=stable">}}下载 x64{{</button>}}

{{<button href="https://update.ryujinx.app/download/query?os=linuxai&arch=arm64&rc=stable">}}下载 ARM{{</button>}}

{{% /columns %}}

## 什么是 Ryujinx Prod Keys？

Ryujinx Prod Keys（生产密钥）是 Ryujinx 解密并运行 Nintendo Switch 游戏所必需的加密密钥。它们来源于 Switch 硬件的安全/加密流程；没有这些密钥，游戏文件将保持加密状态，模拟器无法读取或运行。

**关于 Prod Keys 的要点：**

- **解密**：用于解密被保护的游戏文件。
- **合规**：应从你自己的 Switch 中提取；分发密钥通常是违法的。
- **固件兼容**：固件更新可能导致密钥版本更新，请保持二者匹配。

为在 PC 与其他设备上获得更流畅的体验，Ryujinx 需要相互兼容的 prod keys 与固件。使用下方（NEW）标注的 prod keys 与固件可显著降低卡顿、提升流畅度。

## Ryujinx Prod Keys

| 版本   | 链接 |
| :----: | :--: |
| v20.3.0 | **[DOWNLOAD](/prodkeys/ProdKeys_v20.3.0.zip)** |
| v20.2.0 | **[DOWNLOAD](/prodkeys/ProdKeys_v20.2.0.zip)** |
| V20.1.5 | **[DOWNLOAD](/prodkeys/ProdKeys_v20.1.5.zip)** |
| V20.1.1 | **[DOWNLOAD](/prodkeys/ProdKeys_v20.1.1.zip)** |
| V20.1.0 | **[DOWNLOAD](/prodkeys/ProdKeys_v20.1.0.zip)** |
| V20.0.1 | **[DOWNLOAD](/prodkeys/ProdKeys_v20.0.1.zip)** |
| V20.0.0 | **[DOWNLOAD](/prodkeys/ProdKeys_v20.0.0.zip)** |
| V19.0.1 | **[DOWNLOAD](/prodkeys/ProdKeys_v19.0.1.zip)** |
| V19.0.0 | **[DOWNLOAD](/prodkeys/ProdKeys_v19.0.0.zip)** |
| V18.1.0 | **[DOWNLOAD](/prodkeys/ProdKeys_v18.1.0.zip)** |
| V18.0.1 | **[DOWNLOAD](/prodkeys/ProdKeys_v18.0.1.zip)** |
| V18.0.0 | **[DOWNLOAD](/prodkeys/ProdKeys_v18.0.0.zip)** |
| V17.0.1 | **[DOWNLOAD](/prodkeys/ProdKeys_v17.0.1.zip)** |
| V17.0.0 | **[DOWNLOAD](/prodkeys/ProdKeys_v17.0.0.zip)** |
| V16.1.0 | **[DOWNLOAD](/prodkeys/ProdKeys_v16.1.0.zip)** |
| V16.0.3 | **[DOWNLOAD](/prodkeys/ProdKeys_v16.0.3.zip)** |
| V16.0.2 | **[DOWNLOAD](/prodkeys/ProdKeys_v16.0.2.zip)** |
| V16.0.1 | **[DOWNLOAD](/prodkeys/ProdKeys_v16.0.1.zip)** |
| V16.0.0 | **[DOWNLOAD](/prodkeys/ProdKeys_v16.0.0.zip)** |

## Ryujinx 固件

Ryujinx 固件指从 Nintendo Switch 主机提取的系统软件文件，模拟器需要它们来复现 Switch 的操作环境，许多游戏依赖这些模块与库才能正常运行。

| 版本   | 文件大小 | 链接 |
| ------ | -------- | ---- |
| v20.3.0 | 340MB | [DOWNLOAD](https://github.com/THZoria/NX_Firmware/releases/download/20.3.0/Firmware.20.3.0.zip) |
| v20.2.0 | 340MB | [DOWNLOAD](https://github.com/THZoria/NX_Firmware/releases/download/20.2.0/Firmware.20.2.0.zip) |
| V20.1.5 | 340MB | [DOWNLOAD](https://github.com/THZoria/NX_Firmware/releases/download/20.1.5/Firmware.20.1.5.zip) |
| v20.1.1 | 340MB | [DOWNLOAD](https://github.com/THZoria/NX_Firmware/releases/download/20.1.1/Firmware.20.1.1.zip) |
| v20.1.0 | 340MB | [DOWNLOAD](https://github.com/THZoria/NX_Firmware/releases/download/20.1.0/Firmware.20.1.0.zip) |
| v20.0.1 | 339MB | [DOWNLOAD](https://github.com/THZoria/NX_Firmware/releases/download/20.0.1/Firmware.20.0.1.zip) |
| v20.0.0 | 339MB | [DOWNLOAD](https://github.com/THZoria/NX_Firmware/releases/download/20.0.0/Firmware.20.0.0.zip) |
| v19.0.1 | 322MB | [DOWNLOAD](https://github.com/THZoria/NX_Firmware/releases/download/19.0.1/Firmware.19.0.1.zip) |
| v19.0.0 | 322MB | [DOWNLOAD](https://github.com/THZoria/NX_Firmware/releases/download/19.0.0/Firmware.19.0.0.zip) |
| v18.1.0 | 320MB | [DOWNLOAD](https://github.com/THZoria/NX_Firmware/releases/download/18.1.0/Firmware.18.1.0.zip) |
| v18.0.1 | 323MB | [DOWNLOAD](https://github.com/THZoria/NX_Firmware/releases/download/18.0.1/Firmware.18.0.1.zip) |
| v18.0.0 | 323MB | [DOWNLOAD](https://github.com/THZoria/NX_Firmware/releases/download/18.0.0/Firmware.18.0.0.zip) |
| v17.0.1 | 323MB | [DOWNLOAD](https://github.com/THZoria/NX_Firmware/releases/download/17.0.1/Firmware.17.0.1.zip) |
| v17.0.0 | 323MB | [DOWNLOAD](https://github.com/THZoria/NX_Firmware/releases/download/17.0.0/Firmware.17.0.0.zip) |
| v16.1.0 | 325MB | [DOWNLOAD](https://github.com/THZoria/NX_Firmware/releases/download/16.1.0/Firmware.16.1.0.zip) |
| v16.0.3 | 325MB | [DOWNLOAD](https://github.com/THZoria/NX_Firmware/releases/download/16.0.3/Firmware.16.0.3.zip) |
| v16.0.2 | 325MB | [DOWNLOAD](https://github.com/THZoria/NX_Firmware/releases/download/16.0.2/Firmware.16.0.2.zip) |
| v16.0.1 | 325MB | [DOWNLOAD](https://github.com/THZoria/NX_Firmware/releases/download/16.0.1/Firmware.16.0.1.zip) |
| v16.0.0 | 325MB | [DOWNLOAD](https://github.com/THZoria/NX_Firmware/releases/download/16.0.0/Firmware.16.0.0.zip) |
| v15.0.1 | 322MB | [DOWNLOAD](https://github.com/THZoria/NX_Firmware/releases/download/15.0.1/Firmware.15.0.1.zip) |
| v15.0.0 | 322MB | [DOWNLOAD](https://github.com/THZoria/NX_Firmware/releases/download/15.0.0/Firmware.15.0.0.zip) |

**固件要点：**

- **游戏兼容**：许多游戏依赖固件中的关键库与功能。
- **更新与特性**：较新的固件可能带来更好的兼容性与新功能。
- **获取与合规**：与 Prod Keys 一样，应从你自己的 Switch 中提取。

固件更新通常对新作支持至关重要。

## 如何获取 Ryujinx 的 Prod Keys？

需要从你自己的 Nintendo Switch 中提取。这要求设备可运行自制固件（如 Atmosphère）。

**重要提示**：请仅从你本人拥有的 Switch 中提取，不要从互联网下载，以保证合规。

### 提取步骤概览

- 准备工具：可刷 CFW 的 Switch、SD 卡、Atmosphere、（可选）Hekate、Lockpick_RCM。
- 安装并运行 CFW：进入 RCM，注入 Payload。
- 使用 Lockpick_RCM 提取：生成 prod.keys/title.keys 到 SD 卡。
- 复制到电脑：通常放置于 Ryujinx > system > keys。
- 启动 Ryujinx 验证密钥是否被识别。

### 将 prod.keys 放在何处？

- Windows：C:\\Users\\[用户名]\\AppData\\Roaming\\Ryujinx\\system
- Linux：/home/[用户名]/.config/Ryujinx/system
- macOS：/Users/[用户名]/Library/Application Support/Ryujinx/system

## 如何在 Ryujinx 安装固件？

1) 获取固件文件（从你自己的 Switch 提取，通常为 .zip 或已解包目录）。
2) 启动 Ryujinx → Tools → Install Firmware → 从 XCI/ZIP 或目录安装。
3) 选择固件文件并安装，完成后可在系统信息中查看版本。

### PC 配置建议

- 最低：Windows 10+/Linux/macOS 11+；4 核 x86-64（AVX2）；8GB 内存；支持 Vulkan/OpenGL 4.5 的独显/核显。
- 推荐：6 核 CPU；更强 GPU（如 GTX 1060/RTX 2060、RX 5600）；16GB 内存。

其它：需要最新固件与密钥、充足的存储空间，建议使用兼容手柄。

## 常见问题（FAQ）

### Ryujinx 是否支持 NSP？
支持。

### Ryujinx 是否安全？
只要从官网或可信来源下载，一般是安全的。

## 结语

本文提供了可用于低配设备的 Ryujinx prod keys、title keys 与固件，并给出了提取与安装说明。



