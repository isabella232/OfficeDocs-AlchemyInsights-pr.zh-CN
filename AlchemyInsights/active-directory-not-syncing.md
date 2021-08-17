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
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: d4615d335b9aeef69148cd93ff9f44bec6d7d876
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314194"
---
# <a name="active-directory-not-syncing"></a>Active Directory 未同步

如果您收到同步错误（如"最近未同步"）或注意到 Office 管理门户中的目录同步状态显示"上次同步时间超过 3 天"，可能是 AADConnect 的设置不正确或权限不足，无法执行同步。  

使用快速设置重新安装 AADConnect 可能会快速解决问题：

1. [下载最新版本的 AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771)。

2. [按照快速安装的说明进行操作](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)。

Azure AD Connect 必须安装在 Windows Server 2012 或以上版本。 服务器必须加入域，并且可以是域控制器或成员服务器。 有关 Azure AD 要求连接先决条件的完整列表，请查看[Prerequisites for Azure AD 连接](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-prerequisites)。

有关 AADConnect 服务帐户的详细信息，请参阅 [Azure AD Connect：帐户和权限](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)。
