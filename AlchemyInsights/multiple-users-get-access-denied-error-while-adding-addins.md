---
title: 在 Outlook 中添加加载项时，多个用户收到“拒绝访问”错误
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2020
ms.locfileid: "45397693"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>在 Outlook 中添加加载项时，多个用户收到“拒绝访问”错误

可以指定组织中的哪些管理员有权安装和管理适用于 Outlook 的加载项。 还可以指定组织中的哪些用户有权安装和管理供其自己使用的加载项。

有关详细信息，请参阅[指定可安装和管理 Outlook 加载项的管理员和用户](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)。

若要验证是否已成功为用户分配权限，请将 <Role Name> 替换为要验证的角色的名称，然后在 Exchange Online PowerShell 中运行以下命令：

Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers

此示例演示如何验证向谁分配了为组织安装 Office 应用商店提供的加载项所需的权限。

PowerShell

-Role "Org Marketplace Apps" -GetEffectiveUsers

在结果 Get-ManagementRoleAssignment 中，查看“有效用户”列中的条目。

有关语法和参数的详细信息，请参阅 [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment)。
 