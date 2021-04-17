---
title: Active Directory 未同步
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
- "9001688"
- "3754"
ms.openlocfilehash: 274855457a143cfccd25f9a161ff894882cee9c4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822841"
---
# <a name="active-directory-not-syncing"></a>Active Directory 未同步

如果您收到同步错误（如"最近未同步"）或注意到 Office 管理门户中的目录同步状态显示"上次同步时间超过 3 天"，可能是 AADConnect 的设置不正确或权限不足，无法执行同步。  

使用快速设置重新安装 AADConnect 可能会快速解决问题：

1. [下载最新版本的 AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771)。

2. [按照快速安装的说明进行操作](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)。

有关 AADConnect 服务帐户的详细信息，请参阅 [Azure AD Connect：帐户和权限](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)。
