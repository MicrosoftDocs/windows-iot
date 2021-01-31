---
title: Microsoft Store Access
author: rsameser
ms.author: riameser
ms.date: 1/30/2021
ms.topic: article
ms.prod: windows-iot
ms.technology: iot
description: Learn about the Microsoft Store Access Features of Windows 10 IoT Enterprise.
keywords: Branding, Microsoft Store Access
---

# Microsoft Store Access
You have the option to decide how much access you would like your users to have when it comes to opening the Microsoft Store on Windows 10 IoT Enterprise. Access to the Microsoft store can be blocked or modified achieve a desired customer experience or meet an organization's policy. You can use AppLocker or Group Policy to configure access to Microsoft Store.

> [!NOTE]
> The [Long-Term-Servicing Channel (LTSC)](https://docs.microsoft.com/windows/deployment/update/waas-overview#long-term-servicing-channel) has the store service for updating preinstalled apps, but does not include the Store UI for browsing apps. The [Semi-Annual Channel (SAC)](https://docs.microsoft.com/windows/deployment/update/waas-overview#semi-annual-channel) has both the store service and UI.


## Block Microsoft Store using AppLocker
AppLocker provides policy-based access control management for applications. You can block access to Microsoft Store app with [AppLocker](https://docs.microsoft.com/windows/configuration/stop-employees-from-using-microsoft-store#block-microsoft-store-using-applocker) by creating a rule for packaged apps. You'll give the name of the Microsoft Store app as the packaged app that you want to block from client computers.

For more information on creating an AppLocker rule for app packages,

**To block Microsoft Store using AppLocker:**

1. Type **secpol** in the search bar to find and start AppLocker.

2. In the console tree of the snap-in, click **Application Control Policies**, click **AppLocker**, and then click Packaged app Rules.

3. On the **Action** menu, or by right-clicking on **Packaged app Rules**, click **Create New Rule**.

4. On **Before You Begin**, click **Next**.

5. On **Permissions**, select the action (allow or deny) and the user or group that the rule should apply to, and then click **Next**.

6. On **Publisher**, you can select **Use an installed app package as a reference**, and then click **Select**.

7. On **Select applications**, find and click **Store** under **Applications** column, and then click **OK**. Click **Next**.

8. Optional: On **Exceptions**, specify conditions by which to exclude files from being affected by the rule. This allows you to add exceptions based on the same rule reference and rule scope as you set before. Click **Next**.

> [!TIP]
>
> For more information on creating an AppLocker rule, reference options and setting the scope on packaged app rules, see [create a rule for packaged apps](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-application-control/applocker/create-a-rule-for-packaged-apps).


## Block Microsoft Store using Group Policy
You can also use [Group Policy](https://docs.microsoft.com/windows/configuration/stop-employees-from-using-microsoft-store#block-microsoft-store-using-group-policy) to manage access to Microsoft Store.

**To block Microsoft Store using Group Policy:**

1. Type **gpedit** in the search bar to find and start Group Policy Editor.

2. In the console tree of the snap-in, select **Computer Configuration** > **Administrative Templates** > **Windows Components** > **Store**.

3. In the **Setting pane**, click **Turn off the Store application**, and then click **Edit policy setting**.

4. On the **Turn off the Store application setting** page, click **Enabled**, and then click **OK**.

>[!IMPORTANT]
>
> Enabling **Turn off the Store application** policy turns off app updates from Microsoft Store.

## Block Microsoft Store using configuration service provider
If you have Windows 10 devices in your organization that are managed using a mobile device management (MDM) system, such as Microsoft Intune, you can block access to Microsoft Store app using the following [configuration service providers (CSPs)](https://docs.microsoft.com/windows/configuration/stop-employees-from-using-microsoft-store#block-microsoft-store-using-configuration-service-provider):
* [Policy CSP](https://docs.microsoft.com/windows/client-management/mdm/policy-configuration-service-provider)
* [AppLocker CSP](https://docs.microsoft.com/windows/client-management/mdm/applocker-csp)

For more information, see [Configure an MDM provider](https://docs.microsoft.com/microsoft-store/configure-mdm-provider-microsoft-store-for-business).


## Show private store only using Group Policy
If you're using [Microsoft Store for Business](https://docs.microsoft.com/microsoft-store/microsoft-store-for-business-overview) and you want employees to only see apps you're managing in your private store, you can use [Group Policy](https://docs.microsoft.com/windows/configuration/stop-employees-from-using-microsoft-store#show-private-store-only-using-group-policy) to show only the private store. Microsoft Store app will still be available, but employees can't view or purchase apps. Employees can view and install apps that the admin has added to your organization's private store.

**To show private store only in Microsoft Store app:**

1. Type **gpedit** in the search bar, and then select **Edit group policy (Control panel)** to find and start Group Policy Editor.

2. In the console tree of the snap-in, go to **User Configuration** or **Computer Configuration** > **Administrative Templates** > **Windows Components**, and then click **Store**.

3. Right-click **Only display the private store within the Microsoft Store app** in the right pane, and click **Edit**.

4. On the **Only display the private store within the Microsoft Store app** setting page, click **Enabled**, and then click **OK**.


## App Updates  
There is also a setting for configuring how often the store updates apps and that configuration can be useful when determining when to update applications on your IoT Device.

**To Turn On or Off Update Apps Automatically in Store using Group Policy:**

1. Open Local Group Policy Editor

2. Navigate to **Computer Configuration** > **Administrative Templates** > **Windows Components** > **Store**

3. Double click **Turn off Automatic Download and Install of Updates** policy to edit it.

4. Select **Turn off Automatic Download and Install of updates** policy to edit it.


## Additional Resources
* [Configure access to Microsoft Store](https://docs.microsoft.com/windows/configuration/stop-employees-from-using-microsoft-store#options-to-configure-access-to-microsoft-store)
* [Distribute apps using your private store](https://docs.microsoft.com/microsoft-store/distribute-apps-from-your-private-store)
* [Manage access to private store](https://docs.microsoft.com/microsoft-store/manage-access-to-private-store)
