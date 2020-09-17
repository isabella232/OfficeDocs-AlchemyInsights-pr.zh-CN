---
title: 阻止共享链接上的下载
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000213"
- "5715"
ms.openlocfilehash: 5837013a71648d5d53cd215c3e3489f3de5528d5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685732"
---
# <a name="block-download-on-sharing-links"></a>阻止共享链接上的下载

**阻止下载**适用于指向 Office 文档的**仅查看链接**。 选择此选项后，通过你创建的链接访问文件的用户将不会看到下载、打印或复制文件的选项。

管理员可以通过更改 [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) 或 [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShell cmdlet 中的 `BlockDownloadLinksFileType` 设置来控制是否仅对 Office 文件显示“阻止下载”设置。
