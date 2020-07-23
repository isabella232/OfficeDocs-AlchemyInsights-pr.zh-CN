---
title: 与 SourceAnchor、ProxyAddress 或 UserPrincipalName 存在冲突
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1699"
- "1300022"
ms.openlocfilehash: 826dfe9e5c7d24ff5186a94e1ada4dad536e7edd
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/20/2020
ms.locfileid: "45186095"
---
# <a name="conflicts-with-sourceanchor-proxyaddress-userprincipalname"></a><span data-ttu-id="24f90-102">与 SourceAnchor、ProxyAddress 或 UserPrincipalName 存在冲突</span><span class="sxs-lookup"><span data-stu-id="24f90-102">Conflicts with SourceAnchor, ProxyAddress, UserPrincipalName</span></span>

<span data-ttu-id="24f90-103">如果你在同步期间收到诸如“你的目录中存在已同步且 ProxyAddress 或 UserPrincipalName 相同的对象”的错误，请参阅[诊断和修正“重复属性同步”错误](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors)。</span><span class="sxs-lookup"><span data-stu-id="24f90-103">If you receive errors during a synchronization such as "A synchronized object with the same ProxyAddress or UserPrincipalName exists in your directory", see [Diagnose and remediate duplicated attribute sync errors](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors).</span></span>

<span data-ttu-id="24f90-104">此外，还需考虑启用重复属性复原。</span><span class="sxs-lookup"><span data-stu-id="24f90-104">Also, consider enabling duplicate attribute resiliency.</span></span> <span data-ttu-id="24f90-105">有关详细信息，请参阅[标识同步和重复属性复原](https://aka.ms/duplicateattributeresiliency)。</span><span class="sxs-lookup"><span data-stu-id="24f90-105">For more info, see [Identity synchronization and duplicate attribute resiliency](https://aka.ms/duplicateattributeresiliency).</span></span>