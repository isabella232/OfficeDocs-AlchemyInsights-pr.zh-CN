---
title: 将SharePoint库映射到网络驱动器
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 4b8245c3-a179-4524-ae83-0c22d539c202
ms.openlocfilehash: cd3d7d272552d5cd3f21f41160522001d79339d84a6d2259e1b1868deee66ef0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54087234"
---
# <a name="map-a-sharepoint-library-to-a-network-drive"></a>将SharePoint库映射到网络驱动器

与映射网络驱动器不同，SharePoint新客户端同步文件OneDrive 同步客户端，该客户端提供按需文件。 无需本地存储空间即可访问所有 OneDrive 中的文件。 有关详细信息，请参阅[Sync SharePoint and Teams files with your computer](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88)和 Save disk space with OneDrive Files [On-Demand for Windows 10](https://support.microsoft.com/office/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e)。

如果选择映射驱动器而不是使用新的[OneDrive 同步 客户端](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88)，请确保按照以下步骤操作：

- [对连接到 SharePoint Online 的映射的网络驱动器进行故障排除](/sharepoint/support/administration/troubleshoot-mapped-network-drives)

- [当客户端不支持 TLS 1.2 时，将发生身份验证错误](/sharepoint/troubleshoot/administration/authentication-errors-tls12-support#network-drive-mapped-to-a-sharepoint-library)  

**注意：** 如果使用 Internet Explorer 10 或 Windows 8 Windows 7，并且映射驱动器时收到访问被拒绝或路径不可访问，请安装此修补程序来 [解决此问题。](https://support.microsoft.com/topic/error-when-you-open-a-sharepoint-document-library-in-windows-explorer-or-map-a-network-drive-to-the-library-after-you-install-internet-explorer-10-96e640ba-059f-9b09-bb91-2a0319ee8b1d)