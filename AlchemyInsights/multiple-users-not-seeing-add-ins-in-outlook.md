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
ms.openlocfilehash: a0c272f40044795754ed8630e88e00ed14ea6ad7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47729861"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>多位用户在 Outlook 中看不到加载项

如果你测试 Outlook 加载项，但未显示任何内容，那么在故障排除步骤中，首先要使用 **Get-OrganizationConfig** PowerShell cmdlet 查询 _AppsForOfficeEnabled_ 参数。 如果查询返回了值 **False**，请使用 **Set-OrganizationConfig** cmdlet 将此参数设置为 **True**，使加载项按预期显示。

建议不要将 _AppsForOfficeEnabled_ 参数设置为 **False**。 如果值为 **False**，则将覆盖上面所有的管理和用户角色设置，并阻止组织中的任何用户激活任何新应用。

有关详细信息，请参阅 [指定可安装和管理 Outlook 加载项的管理员和用户](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles)。