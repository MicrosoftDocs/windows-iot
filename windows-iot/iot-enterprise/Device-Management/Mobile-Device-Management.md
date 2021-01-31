---
title: Mobile Device Management
author: rsameser
ms.author: riameser
ms.date: 11/09/2020
ms.topic: article
ms.prod: windows-iot
ms.technology: iot
description: Learn about Mobile Device Management in Windows 10 IoT Enterprise.
keywords: IoT Enterprise, Device Management
---

# Mobile Device Management
Managing a device is now easier than ever on Windows 10 IoT Enterprise. Through [Mobile Device Management (MDM)](https://docs.microsoft.com/windows/client-management/mdm/#learn-about-configuration-service-providers) you have full control which devices are enrolled in various policies.

## What is Mobile Device Management
Windows 10 provides an enterprise management solution to help IT pros manage company security policies and business applications, while avoiding compromise of the users’ privacy on their personal devices. A built-in management component can communicate with the management server.

Check out [What's new in mobile device enrollment and management](https://docs.microsoft.com/windows/client-management/mdm/new-in-windows-mdm-enrollment-management#whatsnew10) to further understand the capabilities that are being offered.

## Mobile Device Management Policies
The MDM security baseline includes policies that cover the following areas:
* Microsoft inbox security technology (not deprecated) such as BitLocker, and Windows Defender SmartScreen. 
* Restricting remote access to devices
* Setting credential requirements for passwords and PINs
* Restricting use of legacy technology
* Legacy technology policies that offer alternative solutions with modern technology

## Learn about Migrating to Mobile Device Management
When an organization wants to move to MDM to manage devices, they should prepare by analyzing their current Group Policy settings to see what they need to transition to MDM management. Microsoft created the [MDM Migration Analysis Tool (MMAT)](https://aka.ms/mmat/) to help. MMAT determines which Group Policies have been set for a target user or computer and then generates a report that lists the level of support for each policy settings in MDM equivalents. For more information, see [MMAT Instructions](https://github.com/WindowsDeviceManagement/MMAT/blob/master/MDM%20Migration%20Analysis%20Tool%20Instructions.pdf).

## Mobile Device Enrollment
Mobile device enrollment is the first phase of enterprise management. The device is configured to communicate with the MDM server using security precautions during the enrollment process. The enrollment service verifies that only authenticated and authorized devices can be managed by their enterprise.

The [enrollment process](https://docs.microsoft.com/windows/client-management/mdm/mobile-device-enrollment) includes the following steps:
1. Discovery of the enrollment endpoint
2. Certificate installation
3. DM Client provisioning

## Additional Resources
* [MDM enrollment of Windows-based devices](https://docs.microsoft.com/windows/client-management/mdm/mdm-enrollment-of-windows-devices)
* [Disabling MDM](https://docs.microsoft.com/windows/client-management/mdm/mobile-device-enrollment#disable-mdm-enrollments)
