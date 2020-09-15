---
title: 电子数据展示导出工具
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 55f29fae0878917eaf2972ba1dfd3c5b8a26ce54
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711085"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>无法安装或运行电子数据展示导出工具？

如果无法安装或运行电子数据展示导出工具以下载搜索结果，请检查以下各项：
  
- 您正在使用的计算机满足以下先决条件：

  - 32 位或 64 位版本的 Windows 7 和更高版本

  - Microsoft .NET Framework 4.7

  - 支持的浏览器：

  - Microsoft Edge

    或

  - Internet Explorer 10 和更高版本

    其他浏览器（如 Google Chrome 和 Mozilla Firefox）不受支持。

- 您的组织可以连接到 Azure 中的终结点，即** \* blob.core.windows.net** (通配符代表导出作业) 的唯一标识符。

- 你已在 Microsoft 365 安全合规中心中分配了导出角色 &amp; 。 默认情况下，此角色仅分配给电子数据展示管理器角色组。 请参阅 [分配电子数据展示权限](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)。

有关详细信息，请参阅 [导出内容搜索结果](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)。
  