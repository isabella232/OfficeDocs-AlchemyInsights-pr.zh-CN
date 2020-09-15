---
title: Active Directory 未同步
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
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697619"
---
# <a name="active-directory-not-syncing"></a>Active Directory 未同步

如果您收到同步错误，例如 "无最近同步"，或注意 Office 管理员门户中的目录同步状态说出 "上次同步时间超过3天前"，可能是 AADConnect 的设置不正确或权限不足，无法执行同步。  

使用快速设置重新安装 AADConnect 可能会快速解决问题：

1. [下载 AADConnect 的最新版本](https://go.microsoft.com/fwlink/?LinkId=615771)。

2. [按照 express 安装的说明进行](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)操作。

有关 AADConnect 服务帐户的详细信息，请参阅 [Azure AD Connect：帐户和权限](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)。
