---
title: Updates
author: rsameser
ms.author: riameser
ms.date: 2/2/2021
ms.topic: article
ms.prod: windows-iot
ms.technology: iot
description: Learn about the Update features of Windows 10 IoT Enterprise.
keywords: IoT Enterprise, Updates
---

# Updates
Connected devices have the challenge of new security threats, updates are an essential tool to address this.

Windows Update Advantage:
- Keeps device up to date with critical security software updates​
- Utilize the Microsoft proven and scalable infrastructure
- Updates can be easily managed and controlled by device owners

Windows 10 IoT Enterprise gives the administrator the power to manage and control updates as per device and organization requirements.

## Control Windows Updates
One of the most common requests from device partners is centered around controlling automatic updates on Windows 10 IoT devices. The nature of IoT devices is such that unexpected disruptions, through something like an unplanned update, can create a bad device experience.

Questions that you should ask when considering how to control Windows updates:
* Is the device scenario such that any disruption of the workflow is unacceptable?
* How are updates validated prior to deployment?
* What is the update user experience on the device itself?

If you have a device where disruption of the user experience isn't acceptable, you should consider limiting updates to only certain hours, disabling automatic updates, or deploying updates either manually or through a controlled third-party [device-management](../Device-Management/Device-Management-Overview.md) solution.

## Limit reboots from updates
You can use the Active Hours Group Policy, MDM, or registry setting to limit updates to only certain hours.

1. Open the Group Policy Editor (gpedit.msc) and navigate to **Computer Configuration\Administrative Templates\Windows Components\Windows Update** and open the **Turn off auto-restart for updates during active hours** policy setting. **Enable** the policy so you can set the start and end times for active hours.
2. Set the **Start** and **End** time to the Active Hours window. For example, set Active Hours to start at 4:00AM and end 2:00AM. This allows the system to reboot from updates between the hours of 2:00 AM and 4:00 AM.

## Disable Automatic Windows Updates
Security and stability are at the core of a successful IoT project, and Windows Update provides updates to ensure Windows 10 IoT Enterprise has the latest applicable security and stability updates. You might, however, have a device scenario where updating Windows has to be handled completely manually. For this type of scenario, we recommend disabling automatic updating through Windows Update. In previous versions of Windows device partners could stop and disable the Windows Update service, but this is no longer the supported method for disabling automatic updates. Windows 10 has a number of policies that allow you to configure Windows Updates in several ways.

To completely disable automatic updating of Windows 10 with Windows Update:
1. Open the Group Policy Editor (gpedit.msc) and navigate to **Computer Configuration\Administrative Templates\Windows Components\Windows update\Configure Automatic Updates**.
2. Explicitly set the policy to **Disabled**. When this setting is set to Disabled, any available updates from Windows Update must be downloaded and installed manually, which you can do in the Settings app under **Update & security > Windows Update**.

## Completely Turn Off Windows Updates
You can configure Windows Update in several ways, and not all policies are applicable to all devices. As a general rule, IoT devices require special attention to the servicing and management strategy to be used on the devices. If your servicing strategy is to disable all Windows Update features, you have two possible approaches. You can turn off updates via [Group Policy](https://docs.microsoft.com/windows-hardware/manufacture/desktop/iot-ent-configure-policy-settings#windows-update-summary) or [Registry](https://docs.microsoft.com/windows/privacy/manage-connections-from-windows-operating-system-components-to-microsoft-services#bkmk-wu).

>[!NOTE]
>
> By setting this policy, it will also stop performing updates from other machines on the local network. To confirm this behavior, you can also turn off [Delivery Optimization](https://docs.microsoft.com/windows/privacy/manage-connections-from-windows-operating-system-components-to-microsoft-services#28-delivery-optimization) which is the subsystem for getting updates from others on your local network.

## Prevent drivers from being installed via Windows Update
Sometimes drivers installed from Windows Update can cause issues with a device experience. The steps below prohibit Windows Update from downloading and installing new drivers on the device.

1. Open the Group Policy Editor (gpedit.msc) and navigate to **Computer Configuration\Administrative Templates\Windows Components\Windows update\Do not include drivers with Windows Updates**.
2. Enable this policy, which tells Windows to not include drivers with Windows quality updates.

## Additional Resources
* [Update Notifications](../Branding-Features/Update-Notification.md)
* [Device Management](../Device-Management/Device-Management-Overview.md)
