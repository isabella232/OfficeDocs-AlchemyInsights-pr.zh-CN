---
title: 多位用户在 Outlook 中看不到加载项
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 850df2cb349f9a751def3d59fb665670e70e493daba56a88821afcef9c48ffa8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54011794"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>多位用户在 Outlook 中看不到加载项

如果你测试 Outlook 加载项，但未显示任何内容，那么在故障排除步骤中，首先要使用 **Get-OrganizationConfig** PowerShell cmdlet 查询 _AppsForOfficeEnabled_ 参数。 如果查询返回了值 **False**，请使用 **Set-OrganizationConfig** cmdlet 将此参数设置为 **True**，使加载项按预期显示。

不建议将 _AppsForOfficeEnabled_ 参数设置为 **False**。**False** 值将替代上述所有管理和用户角色设置，并阻止组织中的任何用户激活任何新应用。

有关详细信息，请参阅 [指定可安装和管理 Outlook 加载项的管理员和用户](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles)。