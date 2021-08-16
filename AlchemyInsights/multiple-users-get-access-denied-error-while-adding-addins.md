---
title: 在 Outlook 中添加加载项时，多个用户收到“拒绝访问”错误
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 5e5f881ad72d2a0f76c8659d6b1044bf6a18464fa8d65c079e44eb1a2afd4431
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54065382"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>在 Outlook 中添加加载项时，多个用户收到“拒绝访问”错误

你可以指定组织中的哪些管理员有权安装和管理适用于 Outlook 的加载项。也可以指定组织中的哪些用户有权安装和管理其自用的加载项。

有关详细信息，请参阅[指定可安装和管理 Outlook 加载项的管理员和用户](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)。

若要验证是否已成功为用户分配权限，请将 <Role Name> 替换为要验证的角色的名称，然后在 Exchange Online PowerShell 中运行以下命令：

Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers

此示例演示如何验证向谁分配了为组织安装 Office 应用商店提供的加载项所需的权限。

PowerShell

-Role "Org Marketplace Apps" -GetEffectiveUsers

在结果 Get-ManagementRoleAssignment 中，查看“有效用户”列中的条目。

有关语法和参数的详细信息，请参阅 [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment)。
 