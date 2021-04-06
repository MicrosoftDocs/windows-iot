---
title: Reduce Disk Footprint - Removable OS Packages
author: rsameser
ms.author: riameser
ms.date: 4/2/2021
ms.topic: article
ms.prod: windows-iot
ms.technology: iot
description: Learn about how to optimize your disk footprint through the removable OS package feature.
keywords: IoT Enterprise, Disk Footprint, Removable Packages, OS Optimization
---

# Reduce Disk Footprint: Removable OS Packages
One way of optimizing your device is through having a reduced disk footprint. We are excited to announce a new feature that will allow you to remove specifically marked OS packages that not be needed for your scenario.

Package Types Include:
* Drivers & Tools
  * [DVD Boot Environment](#dvd=Boot Environment)
* Built-in Apps
* Application Management
  * [Accounts Control Experience Modal](#accounts-control-experience-modal)
  * [App Management UEV](#app-management-uev)
* Biometrics
  *[Bio Enrollment UX](#bio-enrollment-ux)
* Media
* Language
* Fonts


>[!NOTE]
>
> This action cannot be undone, device must be re-imaged to recover removed package

### Explanation of columns

| Name | Description |
|--|--|
| **Removable Package** | Key (internal) name of the service |
| **Description** | The package's description. |
| **Installation** | *Always installed*: Package is installed on Windows 10 IoT Enterprise. |
| **Recommendation** | Microsoft recommendation/advice about removing this package on Windows 10 IoT Enterprise. |
| **Comments** | Additional explanation |

## Accounts Control Experience Modal
| Name | Description |
|--|--|
| **Accounts Control Experience Modal** | Microsoft-Composable-PlatformExtension-AccountsCOntrolExperienceModal|
| **Description** | TBD |
| **Installation** | *Always installed*: Package is installed on Windows 10 IoT Enterprise. |
| **Recommendation** | Microsoft recommendation/advice about removing this package on Windows 10 IoT Enterprise. |
| **Comments** | Additional explanation |

## App Management UEV
| Name | Description |
|--|--|
| **AppManagement_UEV** | Microsoft-Windows-AppManagement-UEV |
| **Description** | User Experience Virtualization (UE-V) |
| **Installation** | *Always installed*: Package is installed on Windows 10 IoT Enterprise. |
| **Recommendation** | Microsoft recommendation/advice about removing this package on Windows 10 IoT Enterprise. |
| **Comments** | Additional explanation |

## Bio Enrollment UX
| Name | Description |
|--|--|
| **BioEnrollment_UX** | Microsoft-Windows-BioEnrollment-UX |
| **Description** | Windows Hello Setup UI |
| **Installation** | *Always installed*: Package is installed on Windows 10 IoT Enterprise. |
| **Recommendation** | Microsoft recommendation/advice about removing this package on Windows 10 IoT Enterprise. |
| **Comments** | Additional explanation |

## DVD Boot Environment
| Name | Description |
|--|--|
| **BootEnvironment_Dvd** | Microsoft-Windows-BootEnvironment_Dvd |
| **Description** | DVD boot configuration |
| **Installation** | *Always installed*: Package is installed on Windows 10 IoT Enterprise. |
| **Recommendation** | Microsoft recommendation/advice about removing this package on Windows 10 IoT Enterprise. |
| **Comments** | Additional explanation |

## Common Regulated Packages
| Name | Description |
|--|--|
| **Common_RegulatedPackages** | Microsoft-Media-Foundation, Microsoft-Windows-Media-Format, Microsoft-Windows-Media-Streaming, Microsoft-WIndows-MediaPlayback-OC, Microsoft-Windows-Portable-Devices, Microsoft-Windows-WebcamExperience, Microsoft-Windows-WinSATMediaFiles |
| **Description** | [Media Features](https://support.microsoft.com/topic/media-feature-pack-for-windows-10-n-may-2020-ebbdf559-b84c-0fc2-bd51-e23c9f6a4439) |
| **Installation** | *Always installed*: Package is installed on Windows 10 IoT Enterprise. |
| **Recommendation** | Microsoft recommendation/advice about removing this package on Windows 10 IoT Enterprise. |
| **Comments** | Additional explanation |

## Computer Manager Launcher
| Name | Description |
|--|--|
| **ComputerManagerLauncher** | Microsoft-Windows-ComputerManagerLauncher |
| **Description** | Computer Management System Tool |
| **Installation** | *Always installed*: Package is installed on Windows 10 IoT Enterprise. |
| **Recommendation** | Microsoft recommendation/advice about removing this package on Windows 10 IoT Enterprise. |
| **Comments** | Additional explanation |

## Disk Defragmenter UI
| Name | Description |
|--|--|
| **Defrag_UI** | Microsoft-Windows-Defrag-UI |
| **Description** | Disk Defragmenter Admin UI |
| **Installation** | *Always installed*: Package is installed on Windows 10 IoT Enterprise. |
| **Recommendation** | Microsoft recommendation/advice about removing this package on Windows 10 IoT Enterprise. |
| **Comments** | Additional explanation |

## Desktop File Explorer
| Name | Description |
|--|--|
| **DesktopFileExplorer** | Microsoft-Windows-DesktopFileExplorer |
| **Description** | File Explorer for system app |
| **Installation** | *Always installed*: Package is installed on Windows 10 IoT Enterprise. |
| **Recommendation** | Microsoft recommendation/advice about removing this package on Windows 10 IoT Enterprise. |
| **Comments** | Additional explanation |

## Fonts
| Name | Description |
|--|--|
| **Fonts_DesktopFonts_NonLeanSupplement** | Microsoft-OneCore-Fonts-DesktopFonts-NonLeanSupplement |
| **Description** | Additional Chinese, Japanese and Korean fonts |
| **Installation** | *Always installed*: Package is installed on Windows 10 IoT Enterprise. |
| **Recommendation** | Microsoft recommendation/advice about removing this package on Windows 10 IoT Enterprise. |
| **Comments** | Additional explanation |

## Language Features
| Name | Description |
|--|--|
| **LanguageFeatures_WordBreaking_Common-legacy** | LanguageFeatures_WordBreaking_Common-legacy |
| **Description** | Legacy neutral word breaker, should only be needed in very rare app compat scenarios |
| **Installation** | *Always installed*: Package is installed on Windows 10 IoT Enterprise. |
| **Recommendation** | Microsoft recommendation/advice about removing this package on Windows 10 IoT Enterprise. |
| **Comments** | Additional explanation |

## Microsoft Edge Dev Tools Client
| Name | Description |
|--|--|
| **MicrosoftEdgeDevToolsClient** | Microsoft-Windows-MicrosoftEdgeDevToolsClient |
| **Description** | Microsoft Edge Developer Tools |
| **Installation** | *Always installed*: Package is installed on Windows 10 IoT Enterprise. |
| **Recommendation** | Microsoft recommendation/advice about removing this package on Windows 10 IoT Enterprise. |
| **Comments** | Additional explanation |

## Miracast Transmitter
| Name | Description |
|--|--|
| **Miracast_Transmitter** | Microsoft-OneCore-Miracast_Transmitter|
| **Description** | Miracast driver |
| **Installation** | *Always installed*: Package is installed on Windows 10 IoT Enterprise. |
| **Recommendation** | Microsoft recommendation/advice about removing this package on Windows 10 IoT Enterprise. |
| **Comments** | Additional explanation |

## Mobile PC Client
| Name | Description |
|--|--|
| **MobilePC_Client** | Microsoft-Windows-MobilePC-Client-Basic |
| **Description** | Windows Mobility Center |
| **Installation** | *Always installed*: Package is installed on Windows 10 IoT Enterprise. |
| **Recommendation** | Microsoft recommendation/advice about removing this package on Windows 10 IoT Enterprise. |
| **Comments** | Additional explanation |

## MultiMedia ACX
| Name | Description |
|--|--|
| **Multimedia_Acx** | Microsoft-OneCore-Multimedia-Acx |
| **Description** | ACX Audio Class Extension for WDF, based audio drivers |
| **Installation** | *Always installed*: Package is installed on Windows 10 IoT Enterprise. |
| **Recommendation** | Microsoft recommendation/advice about removing this package on Windows 10 IoT Enterprise. |
| **Comments** | Additional explanation |

## Net Profiles UX
| Name | Description |
|--|--|
| **NetProfilesUX** | Microsoft-Windows-NetProfilesUX |
| **Description** | Network and Sharing Center control panel |
| **Installation** | *Always installed*: Package is installed on Windows 10 IoT Enterprise. |
| **Recommendation** | Microsoft recommendation/advice about removing this package on Windows 10 IoT Enterprise. |
| **Comments** | Additional explanation |

## One Core Storage Drivers
| Name | Description |
|--|--|
| **OneCore_SD** | Microsoft-OneCore-SD |
| **Description** | SD storage drivers |
| **Installation** | *Always installed*: Package is installed on Windows 10 IoT Enterprise. |
| **Recommendation** | Microsoft recommendation/advice about removing this package on Windows 10 IoT Enterprise. |
| **Comments** | Additional explanation |

## Protected Environment Printer Drivers
| Name | Description |
|--|--|
| **PEAuth_OneCore** | Microsoft-Windows-PEAuth-OneCore|
| **Description** | [Protected Environment service](https://docs.microsoft.com/windows/win32/medfound/protected-media-path#protected-environment) for protecting DRM (Digital Rights Management) contents |
| **Installation** | *Always installed*: Package is installed on Windows 10 IoT Enterprise. |
| **Recommendation** | Microsoft recommendation/advice about removing this package on Windows 10 IoT Enterprise. |
| **Comments** | Additional explanation |

## Printer Drivers
| Name | Description |
|--|--|
| **Printer_Drivers** | Microsoft-Windows-Printer-Drivers |
| **Description** | Printer drivers |
| **Installation** | *Always installed*: Package is installed on Windows 10 IoT Enterprise. |
| **Recommendation** | Microsoft recommendation/advice about removing this package on Windows 10 IoT Enterprise. |
| **Comments** | Additional explanation |

## Printing Premium Tools
| Name | Description |
|--|--|
| **Printing_PremiumTools** | Microsoft-Windows-Printing-PremiumTools |
| **Description** | Printing Premium Tools Collection |
| **Installation** | *Always installed*: Package is installed on Windows 10 IoT Enterprise. |
| **Recommendation** | Microsoft recommendation/advice about removing this package on Windows 10 IoT Enterprise. |
| **Comments** | Additional explanation |

## Recovery Drive
| Name | Description |
|--|--|
| **RecoveryDrive** | Microsoft-Windows-RecoveryDrive |
| **Description** | Recovery media creator |
| **Installation** | *Always installed*: Package is installed on Windows 10 IoT Enterprise. |
| **Recommendation** | Microsoft recommendation/advice about removing this package on Windows 10 IoT Enterprise. |
| **Comments** | Additional explanation |

## Remote Desktop Services
| Name | Description |
|--|--|
| **RemoteDesktopServices_Collaboration** | Microsoft-OneCore-RemoteDesktopServices-Collaboration |
| **Description** | Windows Desktop Sharing |
| **Installation** | *Always installed*: Package is installed on Windows 10 IoT Enterprise. |
| **Recommendation** | Microsoft recommendation/advice about removing this package on Windows 10 IoT Enterprise. |
| **Comments** | Additional explanation |

## Screen Savers
| Name | Description |
|--|--|
| **ScreenSavers** | Microsoft-Windows-ScreenSavers-3D |
| **Description** | 3D screen savers |
| **Installation** | *Always installed*: Package is installed on Windows 10 IoT Enterprise. |
| **Recommendation** | Microsoft recommendation/advice about removing this package on Windows 10 IoT Enterprise. |
| **Comments** | Additional explanation |

## SDK Tools
| Name | Description |
|--|--|
| **SDKTools** | Microsoft-Windows-SDKTools |
| **Description** | SDK tools including regsvr32.exe, regini.exe and debugger engine |
| **Installation** | *Always installed*: Package is installed on Windows 10 IoT Enterprise. |
| **Recommendation** | Microsoft recommendation/advice about removing this package on Windows 10 IoT Enterprise. |
| **Comments** | Additional explanation |

## Sensor Data Service
| Name | Description |
|--|--|
| **SensorDataService** | Microsoft-Windows-SensorDataService |
| **Description** | Legacy camera and image integration service to support Windows Hello for devices using old IR cameras |
| **Installation** | *Always installed*: Package is installed on Windows 10 IoT Enterprise. |
| **Recommendation** | Microsoft recommendation/advice about removing this package on Windows 10 IoT Enterprise. |
| **Comments** | Additional explanation |

## Shell Wallpaper
| Name | Description |
|--|--|
| **Shell_Wallpaper** | Microsoft-Windows-Shell-Wallpaper-Common|
| **Description** | Wallpapers|
| **Installation** | *Always installed*: Package is installed on Windows 10 IoT Enterprise. |
| **Recommendation** | Microsoft recommendation/advice about removing this package on Windows 10 IoT Enterprise. |
| **Comments** | Additional explanation |

## Shell Options
| Name | Description |
|--|--|
| **ShellOptions** | Microsoft-Windows-ShellOptions |
| **Description** | Calc.exe, Character Map |
| **Installation** | *Always installed*: Package is installed on Windows 10 IoT Enterprise. |
| **Recommendation** | Microsoft recommendation/advice about removing this package on Windows 10 IoT Enterprise. |
| **Comments** | Additional explanation |

## Snipping Tool
| Name | Description |
|--|--|
| **SnippingTool** | Microsoft-Windows-SnippingTool |
| **Description** | Snipping Tool |
| **Installation** | *Always installed*: Package is installed on Windows 10 IoT Enterprise. |
| **Recommendation** | Microsoft recommendation/advice about removing this package on Windows 10 IoT Enterprise. |
| **Comments** | Additional explanation |

## Device Settings
| Name | Description |
|--|--|
| **SystemSettings_Devices** | Microsoft-OneCore-SystemSettings-Devices |
| **Description** | Settings handler - Devices |
| **Installation** | *Always installed*: Package is installed on Windows 10 IoT Enterprise. |
| **Recommendation** | Microsoft recommendation/advice about removing this package on Windows 10 IoT Enterprise. |
| **Comments** | Additional explanation |


## Network and Mobile Settings
| Name | Description |
|--|--|
| **SystemSettings_NetworkMobileHanlders** | Microsoft-OneCore-SystemSettings-NetworkMobileHandlers |
| **Description** | Settings handler - Network and Mobile |
| **Installation** | *Always installed*: Package is installed on Windows 10 IoT Enterprise. |
| **Recommendation** | Microsoft recommendation/advice about removing this package on Windows 10 IoT Enterprise. |
| **Comments** | Additional explanation |

## User Account Settings
| Name | Description |
|--|--|
| **SystemSettings_UserAccount** | Microsoft-OneCore-SystemSettings-UserAccount |
| **Description** | Settings handler - User Accounts |
| **Installation** | *Always installed*: Package is installed on Windows 10 IoT Enterprise. |
| **Recommendation** | Microsoft recommendation/advice about removing this package on Windows 10 IoT Enterprise. |
| **Comments** | Additional explanation |

## Window Tab Manager
| Name | Description |
|--|--|
| **UI_Shell_WindowTabManager** | Microsoft-Windows-UI-Shell-WindowTabManager |
| **Description** | TBD |
| **Installation** | *Always installed*: Package is installed on Windows 10 IoT Enterprise. |
| **Recommendation** | Microsoft recommendation/advice about removing this package on Windows 10 IoT Enterprise. |
| **Comments** | Additional explanation |

## USB Connector Manager
| Name | Description |
|--|--|
| **UsbConnectorManager** | Microsoft-OneCore-Connectivity-UsbConnectorManager, Microsoft-OneCore-Connectivity-UsbFunction |
| **Description** | Required for systems with USB-C connectors, and systems that support USB device/function role |
| **Installation** | *Always installed*: Package is installed on Windows 10 IoT Enterprise. |
| **Recommendation** | Microsoft recommendation/advice about removing this package on Windows 10 IoT Enterprise. |
| **Comments** | Additional explanation |

## Calculator App
| Name | Description |
|--|--|
| **win32calc** | Microsoft-Windows-win32calc |
| **Description** | Win32 Calculator |
| **Installation** | *Always installed*: Package is installed on Windows 10 IoT Enterprise. |
| **Recommendation** | Microsoft recommendation/advice about removing this package on Windows 10 IoT Enterprise. |
| **Comments** | Additional explanation |

## Windows 3D Audio
| Name | Description |
|--|--|
| **Windows_3DAudio_HrtfData** | Microsoft-Windows-3DAudio-HrtfData|
| **Description** | Data files for Windows Sonic spatial audio format |
| **Installation** | *Always installed*: Package is installed on Windows 10 IoT Enterprise. |
| **Recommendation** | Microsoft recommendation/advice about removing this package on Windows 10 IoT Enterprise. |
| **Comments** | Additional explanation |
