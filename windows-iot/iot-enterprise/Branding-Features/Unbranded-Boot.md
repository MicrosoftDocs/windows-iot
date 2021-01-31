---
title: Unbranded Boot
author: rsameser
ms.author: riameser
ms.date: 1/30/2021
ms.topic: article
ms.prod: windows-iot
ms.technology: iot
description: Learn about the Unbranded Boot Feature in Windows 10 IoT Enterprise.
keywords: Branding, Unbranded Boot
---

# Unbranded Boot
You can suppress Windows elements that appear when Windows starts or resumes and can suppress the crash screen when Windows encounters an error that it cannot recover from. This feature is known as [Unbranded Boot](https://docs.microsoft.com/windows-hardware/customize/enterprise/unbranded-boot). This feature allows you to customize and control the user experience during transitions.

## Turn on Unbranded Boot settings
Unbranded Boot is an optional component and is not enabled by default in Windows 10. It must be enabled prior to configuring. You can turn on Unbranded Boot by using [Control Panel](https://docs.microsoft.com/windows-hardware/customize/enterprise/unbranded-boot#turn-on-unbranded-boot-by-using-control-panel).

> [!NOTE]
>
> If Windows has already been installed you cannot apply a provisioning package to configure Unbranded Boot; instead you must use BDCEdit to configure Unbranded boot if Windows is installed.
>
> BCDEdit is the primary tool for editing the startup configuration and is on your development computer in the %WINDIR%\System32 folder. You have administrator rights for it. BCDEdit is included in a typical Windows Preinstallation Environment (Windows PE) 4.0. You can download it from the [BCDEdit Commands for Boot Environment](https://docs.microsoft.com/en-us/previous-versions/windows/hardware/design/dn653986(v=vs.85)) in the Microsoft Download Center if needed.

## Configure Unbranded Boot
There are multiple ways to configure Unbranded Boot. Use the method that is appropriate for your organization.

* [BCDEdit](https://docs.microsoft.com/windows-hardware/customize/enterprise/unbranded-boot#configure-unbranded-boot-settings-at-runtime-using-bcdedit)
* [Unattend](https://docs.microsoft.com/windows-hardware/customize/enterprise/unbranded-boot#configure-unbranded-boot-using-unattend)
* [Deployment Image Servicing and Management (DISM)](https://docs.microsoft.com/windows-hardware/customize/enterprise/unbranded-boot#customize-the-boot-screen-using-windows-configuration-designer-and-deployment-image-servicing-and-management-dism)


## Additional Resources
* [Replace the startup logo](https://docs.microsoft.com/windows-hardware/customize/enterprise/unbranded-boot#replace-the-startup-logo)
