---
title: UPN 同步已禁用
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 33bc7e30d41ff70e2ce55d946202acf45dbcb0f2
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726094"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="113c0-102">UPN 同步已禁用</span><span class="sxs-lookup"><span data-stu-id="113c0-102">UPN sync disabled</span></span>

<span data-ttu-id="113c0-103">如果已开始在2016年3月30日之前同步到 Azure AD，请运行以下 Azure AD PowerShell cmdlet，仅为您的组织启用 UPN 软匹配：</span><span class="sxs-lookup"><span data-stu-id="113c0-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="113c0-104">**MsolDirSyncFeature-功能 EnableSoftMatchOnUpn-启用 $True**</span><span class="sxs-lookup"><span data-stu-id="113c0-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="113c0-105">对于在2016年3月30日或之后开始同步到 Azure AD 的组织，将自动启用 UPN 软匹配。</span><span class="sxs-lookup"><span data-stu-id="113c0-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="113c0-106">若要了解有关在 UPN 和其他同步功能上启用软匹配的详细信息，请参阅[AZURE AD Connect sync service 功能](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)。</span><span class="sxs-lookup"><span data-stu-id="113c0-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

