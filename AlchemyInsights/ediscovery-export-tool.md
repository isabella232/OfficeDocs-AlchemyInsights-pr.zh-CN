---
title: 电子数据展示导出工具
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: f7b7e1ae4f1f686fa510403d398c4ff750dbadb9065b8d63701a927eeac52d9b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101292"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>无法安装或运行电子数据展示导出工具？

如果无法安装或运行电子数据展示导出工具来下载搜索结果，请检查以下内容：
  
- 你使用的计算机满足以下先决条件：

  - 32 位或 64 位版本的 Windows 7 和更高版本

  - Microsoft .NET Framework 4.7

  - 支持的浏览器：

  - Microsoft Edge

    或

  - Internet Explorer 10 和更高版本

    其他浏览器（如 Google Chrome 和 Mozilla Firefox）不受支持。

- 你的组织可以连接到 Azure 中的终结点，即 **\* .blob.core.windows.net (** 通配符表示导出作业应用程序的唯一) 。

- 在安全与合规中心内，Microsoft 365 &amp; 导出角色。 默认情况下，仅向电子数据展示管理员角色组分配此角色。 请参阅 [分配电子数据展示权限](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)。

有关详细信息，请参阅导出 [内容搜索结果](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)。

如果要导出超过 10 万个邮箱，则需要使用以下 Powershell 下载导出结果：从  [超过 10 万](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)个邮箱导出结果。