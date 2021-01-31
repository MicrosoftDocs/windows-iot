---
title: Start Prototyping
author: rsameser
ms.author: riameser
ms.date: 1/31/2021
ms.topic: article
ms.prod: windows-iot
ms.technology: iot
description: Learn how to prototype with Windows 10 IoT Enterprise
keywords: IoT Enterprise, Prototype, Hardware, SoCs, Custom Boards, development devices, boards, SOC, SOM, system on chips, Windows IoT
---
# Start Prototyping
This guide will walk you through how to start prototyping Windows 10 IoT Enterprise.

## Step 1: Select hardware
To begin your prototyping journey, you can choose to use your existing hardware to run Windows 10 IoT Enterprise as long as they meet the [requirements](./Hardware_Requirements.md) or you can select a SoC board.

The following boards have been proven to be a great start point for your Windows 10 IoT Enterprise solution. Feel free to choose a specific version based upon your budgetary constraints and technical requirements.

* [Latte Panda](https://www.lattepanda.com/)
* [Intel NuC](https://www.intel.com/content/www/us/en/products/boards-kits/nuc.html)
* [Asus Vivo Mini](https://www.asus.com/us/Mini-PCs/VivoMini-Products/)
* [AAEON Up Squared](https://www.aaeon.com/en/p/iot-gateway-maker-boards-up-squared)
* [Up Board](https://up-board.org/up/specifications/)

**If you are a SoM provider or an ODM and would like to be added to the list below, please send email to winiotentsomhelp@microsoft.com or directly edit this page and submit a pull request.**

## Step 2: Evaluate Edition
To get started, you can leverage the [Windows 10 IoT Enterprise 90 day Evaluation](https://www.microsoft.com/evalcenter/evaluate-windows-10-enterprise). To select which edition of Windows 10 IoT Enterprise you would like to work with, please review [Features by Release](../Features.md).

## Step 3: Deploy an Image
If your board comes with instructions on how to deploy Windows 10 IoT Enterprise, please follow that.
Otherwise, please follow the guide in the [Windows 10 IoT Enterprise Manufacturing Guide](../Commercialization/Manufacturing-Guide.md).

## Step 4: Load an Application
You can choose to port over your existing Windows applications or try out [UWP (Universal Windows Platform)](https://docs.microsoft.com/windows/uwp/get-started/universal-application-platform-guide) applications.

All UWP applications are designed to run on all Windows 10 API compatible platforms, including Windows 10 IoT Enterprise. UWP is one of many ways to create client applications for Windows. UWP apps use WinRT APIs to provide powerful UI and advanced asynchronous features that are ideal for internet-connected devices.

You can either choose an existing UWP application to run or create your own. Feel free to reference our [UWP app samples](https://github.com/microsoft/Windows-universal-samples) in GitHub.

## Step 5: Licensing & Distribution
If you are interested in pursuing your prototype, past the 90 day evaluation period, please reach out to a distributor. Microsoft offers more than 500 Windows IoT and Embedded SKUs. Authorized distributors of Windows IoT products can help you pick the right SKU for your hardware and your budget by leveraging their development experiences, and knowledge, to help you build secure and connected Windows IoT solutions. If you would like to work with one of our distributors, please [select a distributor](https://aka.ms/IoTDistributorList) in your region and contact the distributor directly for more details.

## Additional Resources
* [Windows 10 IoT Enterprise Manufacturing Guide](https://docs.microsoft.com/windows-hardware/manufacture/desktop/iot-ent-overview)
* [Windows Processor Requirements](https://docs.microsoft.com/windows-hardware/design/minimum/windows-processor-requirements)
