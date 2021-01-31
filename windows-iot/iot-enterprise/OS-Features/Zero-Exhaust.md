---
title: Network Service Controls
author: rsameser
ms.author: riameser
ms.date: 1/30/2021
ms.topic: article
ms.prod: windows-iot
ms.technology: iot
description: Learn about the Network Service Controls features of Windows 10 IoT Enterprise.
keywords: IoT Enterprise, zero exhaust, Network service controls
---

# Network Service Controls
Learn how to manage various network service control options in Windows 10 IoT Enterprise. If you want to minimize connections from Windows to Microsoft services, or configure privacy settings, there are a number of [settings](https://docs.microsoft.com/windows/privacy/manage-connections-from-windows-operating-system-components-to-microsoft-services) for consideration. This [list](https://docs.microsoft.com/windows/privacy/manage-connections-from-windows-operating-system-components-to-microsoft-services#settings-for-windows-10-enterprise-edition) displays the network connections to Microsoft services by default and shows you how to configure these settings to control the data that is sent to Microsoft.

>[!NOTE]
>
> Microsoft is [increasing transparency](https://blogs.microsoft.com/on-the-issues/2019/04/30/increasing-transparency-and-customer-control-over-data/) by categorizing the data we collect as required or optional. For more information, see [Changes to Windows diagnostic data](https://docs.microsoft.com/windows/privacy/changes-to-windows-diagnostic-data-collection).


## Zero exhaust
Zero exhaust is defined as no network traffic (diagnostic data or otherwise, such as downloading background images, Windows Updates, etc.) from Windows and inbox applications to public IP addresses unless directly intended by the user.

This allows the enterprise administrators to configure devices where no network communication is initiated by the system without explicit approval.

To prevent Windows from sending any data to Microsoft, follow the these steps:
1. Configure diagnostic data at the Security level
2. Turn off Windows Defender diagnostic data and Microsoft reporting
3. Turn off all of these [connections](https://docs.microsoft.com/windows/privacy/manage-connections-from-windows-operating-system-components-to-microsoft-services#settings-for-windows-10-enterprise-edition)

>[!TIP]
>
> Microsoft strongly recommends customers to not enable zero exhaust, **unless absolutely necessary** as crucial security patches and updates may be missed, leaving devices vulnerable. Instead it is recommended customers manage their network service controls and pick and choose which connections (if any) to disable.


## Additional Resources
* [Manage Settings for Windows 10 IoT Enterprise](https://docs.microsoft.com/windows/privacy/manage-connections-from-windows-operating-system-components-to-microsoft-services#settings-for-windows-10-enterprise-edition)
* [Configure Windows diagnostic data in your organization](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)
* [TPMPolicy CSP](https://docs.microsoft.com/windows/client-management/mdm/tpmpolicy-csp#:~:text=Zero%20exhaust%20is%20defined%20as%20no%20network%20traffic,IP%20addresses%20unless%20directly%20intended%20by%20the%20user.)
