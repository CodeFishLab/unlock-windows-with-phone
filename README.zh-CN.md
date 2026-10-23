<!-- Created by fish on 22 Oct 2026 -->
# Phone Unlock

[English](README.md) | 简体中文

用身边的 iPhone 或 Android 手机解锁 Windows。本仓库只提供发布版下载。

## 下载

在 [Releases](https://github.com/CodeFishLab/unlock-windows-with-phone/releases/latest) 下载最新文件：

- `PhoneUnlock_<版本>_x64_setup.exe`：Windows 安装程序。
- `PhoneUnlock_<版本>_android.apk`：Android App。Windows 中 **About → Android app** 的二维码也会打开这个页面。

## 系统要求

- Windows 10 2004（内部版本 19041）或更高版本，包括 Windows 11，x64。
- 蓝牙支持 BLE Central、受保护的 GATT 访问和广播扫描。
- 使用设有密码的 Windows **Microsoft 账户（MSA）**登录，不支持本地账户。
- Android 手机需 Android 13 或更高版本。iPhone 无需安装 App。

## 在 Windows 上安装

> [!WARNING]
> 如果装有 **3.1.0** 之前的版本，请先在 Windows **设置 → 应用** 中卸载。

1. 运行安装程序。重启后先用平时的密码或 PIN 登录一次，然后选择 **Start setup**。
2. 保存 **Microsoft 账户密码**，不是 PIN。
3. 在 **Status** 页点击 **Open Bluetooth settings** 配对手机，两台设备上的数字一致时才接受。
4. 回到 **Status**，选择手机并点击 **Bind selected device**，确认 **Initial signal threshold**（初始信号阈值）并通过 UAC。

## 设置 Android App

1. 安装 APK。
2. 允许 **附近的设备** 和通知权限，并将电池用量设为 **不受限制**,还需允许自启动和后台运行。
3. 在 App 中启动服务，然后按上面的步骤在 Windows 上配对并绑定手机。

## 卸载

打开 Windows **设置 → 应用**，找到 *Phone Unlock* 并选择 **卸载**。Windows 蓝牙配对会保留，如有需要请在蓝牙设置中移除。

---

基于 [dennis6481/unlock-windows-with-iphone](https://github.com/dennis6481/unlock-windows-with-iphone)，原项目只支持用 iPhone 解锁 Windows。本项目增加了 Android 支持：安装 Phone Unlock App 后，手机会按你选择的解锁策略响应每次解锁请求，还能锁定或关闭电脑。实验性项目，使用风险自负。参见 [MIT 许可证](LICENSE.md)。
