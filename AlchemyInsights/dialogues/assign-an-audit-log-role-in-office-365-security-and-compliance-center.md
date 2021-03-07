---
title: 在 Office 365 安全与合规中心内分配审核日志角色
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/21/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7363"
- "9000722"
ms.openlocfilehash: 0eb470b6c17def5517db2f866ef40898b36662ed
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50509654"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a>在 Office 365 安全与合规中心内分配审核日志角色

若要搜索 Office 365 审核日志，必须在 Exchange Online 中为管理员分配 **仅查看审核日志** 角色或 **审核日志** 角色。 默认情况下，这些角色分配给合规性管理和组织管理角色组。 Office 365 和 Microsoft 365 中的全局管理员将自动添加为组织管理角色组成员。

若要让用户能够使用最低级别权限搜索，可以在 Exchange Online 中创建自定义角色组，添加 **仅供查看审核日志** 或 **审核日志** 角色，然后将用户添加为新角色组的成员。

有关详细信息，请参阅 [在 Exchange Online 中管理角色组](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) 和 [在安全与合规中心中搜索审核日志](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)。