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
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="382bb-102">多位用户在 Outlook 中看不到加载项</span><span class="sxs-lookup"><span data-stu-id="382bb-102">Multiple users not seeing add-ins in Outlook</span></span>

<span data-ttu-id="382bb-103">如果你测试 Outlook 加载项，但未显示任何内容，那么在故障排除步骤中，首先要使用 **Get-OrganizationConfig** PowerShell cmdlet 查询 _AppsForOfficeEnabled_ 参数。</span><span class="sxs-lookup"><span data-stu-id="382bb-103">If you test Outlook add-ins and none show up, as a first troubleshooting step, use the **Get-OrganizationConfig** PowerShell cmdlet to query the _AppsForOfficeEnabled_ parameter.</span></span> <span data-ttu-id="382bb-104">如果查询返回了值 **False**，请使用 **Set-OrganizationConfig** cmdlet 将此参数设置为 **True**，使加载项按预期显示。</span><span class="sxs-lookup"><span data-stu-id="382bb-104">If the query returns a value of **False**, set this parameter to **True** by using the **Set-OrganizationConfig** cmdlet, so add-ins appear as expected.</span></span>

<span data-ttu-id="382bb-105">建议不要将 _AppsForOfficeEnabled_ 参数设置为 **False**。</span><span class="sxs-lookup"><span data-stu-id="382bb-105">We do not recommend that the _AppsForOfficeEnabled_ parameter is set to **False**.</span></span> <span data-ttu-id="382bb-106">如果值为 **False**，则将覆盖上面所有的管理和用户角色设置，并阻止组织中的任何用户激活任何新应用。</span><span class="sxs-lookup"><span data-stu-id="382bb-106">A value of **False** overrides all of the above Administrative and User role settings and prevents any new apps from being activated by any user in the organization.</span></span>

<span data-ttu-id="382bb-107">有关详细信息，请参阅 [指定可安装和管理 Outlook 加载项的管理员和用户](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles)。</span><span class="sxs-lookup"><span data-stu-id="382bb-107">For more information, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span></span>