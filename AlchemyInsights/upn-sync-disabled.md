---
title: UPN 同步已禁用
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 2b1ba772459091ce1a796884997fe2516d0407eb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782141"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="28bd1-102">UPN 同步已禁用</span><span class="sxs-lookup"><span data-stu-id="28bd1-102">UPN sync disabled</span></span>

<span data-ttu-id="28bd1-103">如果你在 2016 年 3 月 30 日之前开始同步到 Azure AD，请运行以下 Azure AD PowerShell cmdlet 以仅为组织启用 UPN 软匹配：</span><span class="sxs-lookup"><span data-stu-id="28bd1-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="28bd1-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span><span class="sxs-lookup"><span data-stu-id="28bd1-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="28bd1-105">对于在 2016 年 3 月 30 日或之后开始同步到 Azure AD 的组织，将自动启用 UPN 软匹配。</span><span class="sxs-lookup"><span data-stu-id="28bd1-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="28bd1-106">若要了解有关在 UPN 和其他同步功能上启用软匹配功能的信息，请参阅 [Azure AD Connect 同步服务功能](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)。</span><span class="sxs-lookup"><span data-stu-id="28bd1-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

