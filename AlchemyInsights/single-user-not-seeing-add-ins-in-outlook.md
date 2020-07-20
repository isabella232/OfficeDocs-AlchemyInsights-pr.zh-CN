---
title: 一名用户在 Outlook 中看不到加载项
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 1f547c3f593b3256bd44f518aacbc36ed1c4c848
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2020
ms.locfileid: "45154548"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a>一名用户在 Outlook 中看不到加载项

该用户属于的角色可能没有正确的 AppsForOfficeEnabled 参数。 请运行以下 cmdlet，检查该用户是否已关联适当的角色：

Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType

有关详细信息，请参阅[指定可安装和管理 Outlook 加载项的管理员和用户](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)。
