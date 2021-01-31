---
title: Secondary Tiles
author: rsameser
ms.author: riameser
ms.date: 1/30/2020
ms.topic: article
ms.prod: windows-iot
ms.technology: iot
description: Learn about the Secondary Microsoft Edge Tiles of Windows 10 IoT Enterprise.
keywords: Branding, Edge Tiles
---

# Secondary Tiles
Secondary tiles allow users to pin specific content and deep links from your app onto their Start menu, providing easy future access to the content within your app.

By adding secondary tiles to your app, you help the user re-engage quickly and efficiently with your app, encouraging them to return more often, thanks to the easy access that secondary tiles provides.

![Screenshot of secondary tiles](media/secondarytiles.png)

## Secondary tiles in relation to primary tiles
Primary app tiles are the Start screen tiles that represent and launch an app. Secondary tiles are associated with a single parent app. They are pinned to the Start menu to provide a user with a consistent and efficient way to launch directly into a frequently used area of the parent app. This can be either a general subsection of the parent app that contains frequently updated content, or a deep link to a specific area in the app.

**Examples of secondary tile scenarios include:**

* Weather updates for a specific city in a weather app
* A summary of upcoming events in a calendar app
* Status and updates from an important contact in a social app
* Specific feeds in an RSS reader
* A music playlist
* A blog

Any frequently changing content that a user wants to monitor is a good candidate for a secondary tile. After the secondary tile is pinned, users can receive at-a-glance updates through the tile and use it to launch directly into the parent app.

**Secondary tiles are similar to primary tiles in many ways**

* They use tile notifications to display rich content.
* They must include a 150 x 150 pixel logo for the default tile content.
* They can optionally include the other logo sizes to enable larger tile sizes.
* They can show notifications and badges.
* They can be rearranged on the Start menu.
* They are automatically deleted when the app is uninstalled.
* Their badge and lock detailed status text can be shown on lock.

**However, secondary tiles differ from primary tiles in some noticeable ways:**

* Users can delete their secondary tiles at any time without deleting the parent app.
* Secondary tiles can be created at run time. App tiles can be created only during installation.
* A flyout prompts the user for confirmation before adding a secondary tile.
* They cannot be programmatically selected for the lock screen through a request to the user. The user must manually add the secondary tile through the Personalize page in PC Settings.

For sending notifications, specific methods are provided for tile and badge updaters and push notification channels used with secondary tiles. These parallel the versions used with primary tiles. For instance, CreateBadgeUpdaterForApplication vs. CreateBadgeUpdaterForSecondaryTile.


## Additional Resources
* [Add image for secondary Microsoft Edge tiles](https://docs.microsoft.com/windows/configuration/start-secondary-tiles)
* [Secondary tiles](https://docs.microsoft.com/windows/uwp/design/shell/tiles-and-notifications/secondary-tiles)
* [Secondary tile guidance](https://docs.microsoft.com/windows/uwp/design/shell/tiles-and-notifications/secondary-tiles-guidance)
* [Pin secondary tiles](https://docs.microsoft.com/windows/uwp/design/shell/tiles-and-notifications/secondary-tiles-pinning)
* [Tile assets](https://docs.microsoft.com/windows/uwp/design/style/app-icons-and-logos)
* [Tile content documentation](https://docs.microsoft.com/windows/uwp/design/shell/tiles-and-notifications/create-adaptive-tiles)
* [Send a local tile notification](https://docs.microsoft.com/windows/uwp/design/shell/tiles-and-notifications/sending-a-local-tile-notification)
