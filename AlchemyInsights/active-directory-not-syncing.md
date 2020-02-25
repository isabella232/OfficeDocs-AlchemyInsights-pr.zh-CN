---
title: Active Directory 未同步
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3abad160ab28922685d235a1fa546105e31757fb
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265129"
---
# <a name="active-directory-not-syncing"></a>Active Directory 未同步

如果您收到同步错误，如 "无最近同步"，或者注意 Office 管理门户中的目录同步状态说出 "上次同步时间超过3天前"，可能是 AADConnect 的设置不正确或不足执行同步的权限。  

使用快速设置重新安装 AADConnect 可能会快速解决问题：

1. [下载 AADConnect 的最新版本](https://go.microsoft.com/fwlink/?LinkId=615771)。

2. [按照 express 安装的说明进行](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)操作。

有关 AADConnect 服务帐户的详细信息，请参阅[AZURE AD Connect：帐户和权限](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)。
