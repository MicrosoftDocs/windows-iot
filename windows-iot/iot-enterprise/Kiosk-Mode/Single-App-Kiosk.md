---
title: Assigned access Single-App Kiosk
author: rsameser
ms.author: riameser
ms.date: 11/09/2020
ms.topic: article
ms.prod: windows-iot
ms.technology: iot
description: Learn about the Single-App Kiosk in Windows 10 IoT Enterprise.
keywords: Kiosk Mode, Single-App
---

# Assigned access single-app kiosk
A single-app kiosk uses the assigned access feature to run a single app above the lock screen. When the kiosk account signs in, the app is launched automatically. The person using the kiosk cannot do anything on the device outside of the kiosk app.


## Benefits of using a single-app kiosk
A single-app kiosk is ideal for public use. Using Shell Launcher, you can configure a kiosk device that runs a Windows desktop application as the user interface. The application that you specify replaces the default shell (explorer.exe) that usually runs when a user logs on. This type of single-app kiosk does not run above the lock screen.

> [!NOTE]
> Assigned access single-app kiosk mode is not supported over a remote desktop connection. Your kiosk users must sign in on the physical device that is set up as a kiosk.

## Configuring your single-app kiosks
You have several options for configuring your single-app kiosk.
* [Locally, in Settings](https://docs.microsoft.com/windows/configuration/kiosk-single-app#local)
* [PowerShell](https://docs.microsoft.com/windows/configuration/kiosk-single-app#powershell)
* [The Kiosk Wizard in Windows Configuration Designer](https://docs.microsoft.com/windows/configuration/kiosk-single-app#wizard)
* [Microsoft Intune or other MDM providers](https://docs.microsoft.com/windows/configuration/kiosk-single-app#mdm)

> [!TIP]
> You can also configure a kiosk account and app for single-app kiosk within [XML in a provisioning package](https://docs.microsoft.com/windows/configuration/lock-down-windows-10-to-specific-apps) by using a [kiosk profile](https://docs.microsoft.com/windows/configuration/lock-down-windows-10-to-specific-apps#profile). Be sure to check the [configuration recommendations](https://docs.microsoft.com/windows/configuration/kiosk-prepare) before you set up your kiosk.

## Additional Resources
* [Guidelines for choosing an app for assigned access](https://docs.microsoft.com/windows/configuration/guidelines-for-assigned-access-app)
* [Kiosk apps for assigned access: Best practices](https://docs.microsoft.com/windows-hardware/drivers/partnerapps/create-a-kiosk-app-for-assigned-access)
