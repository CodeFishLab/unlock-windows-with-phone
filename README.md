<!-- Created by fish on 22 Oct 2026 -->
# Phone Unlock

English | [简体中文](README.zh-CN.md)

Unlock your Windows session with your nearby iPhone or Android phone. This repository hosts the release downloads only.

## Download

Get the latest files from [Releases](https://github.com/CodeFishLab/unlock-windows-with-phone/releases/latest):

- `PhoneUnlock_<version>_x64_setup.exe`: the Windows installer.
- `PhoneUnlock_<version>_android.apk`: the Android app. The QR code under **About → Android app** on Windows opens the same page.

## System requirements

- Windows 10 version 2004 (build 19041) or later, including Windows 11, x64.
- Bluetooth with BLE Central, protected GATT access and advertisement scanning.
- A Windows **Microsoft account (MSA)** with a password. Local accounts are not supported.
- Android phones need Android 13 or later. iPhone needs no app.

## Install on Windows

> [!WARNING]
> If a version earlier than **3.1.0** is installed, uninstall it in Windows **Settings → Apps** first.

1. Run the installer. After restarting, sign in once with your usual password or PIN, then choose **Start setup**.
2. Save your **Microsoft account password**, not your PIN.
3. On **Status**, use **Open Bluetooth settings** to pair your phone. Accept only if the numbers on both devices match.
4. Return to **Status**, select the phone and click **Bind selected device**, then confirm the **Initial signal threshold** and UAC.

## Set up the Android app

1. Install the APK.
2. Allow **Nearby devices** and notifications, and set battery use to **Unrestricted**, also allow auto-start and background activity.
3. Start the service in the app, then pair and bind the phone on Windows as above.

## Uninstall

Open Windows **Settings → Apps**, find *Phone Unlock* and select **Uninstall**. Windows Bluetooth pairing is kept; remove it in Bluetooth settings if desired.

---

Based on [dennis6481/unlock-windows-with-iphone](https://github.com/dennis6481/unlock-windows-with-iphone). This project adds Android support: the Phone Unlock app answers each unlock request under the policy you choose, and can also lock or shut down the PC. Experimental project; use at your own risk. See the [MIT License](LICENSE.md).
