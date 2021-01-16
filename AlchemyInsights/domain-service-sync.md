---
title: 域服务同步
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "7922"
- "7921"
ms.openlocfilehash: b35d3a402bc08a27a818209385c5666b901fa524
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49876513"
---
# <a name="domain-service-synchronization"></a><span data-ttu-id="91066-102">域服务同步</span><span class="sxs-lookup"><span data-stu-id="91066-102">Domain service synchronization</span></span>

<span data-ttu-id="91066-103">Azure Active Directory 域服务 (Azure AD DS) 托管域中的对象和凭据可以在域中本地创建，也可以从 Azure Active Directory (Azure AD) 租户同步。</span><span class="sxs-lookup"><span data-stu-id="91066-103">Objects and credentials in an Azure Active Directory Domain Services (Azure AD DS) managed domain can either be created locally within the domain, or synchronized from an Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="91066-104">首次部署 Azure AD DS 时，将配置并启动自动单向同步以从 Azure AD 复制对象。</span><span class="sxs-lookup"><span data-stu-id="91066-104">When you first deploy Azure AD DS, an automatic one-way synchronization is configured and initiated to replicate the objects from Azure AD.</span></span> <span data-ttu-id="91066-105">此单向同步将继续在后台运行，使 Azure AD DS 托管域保持最新状态以及 Azure AD 的任何更改。</span><span class="sxs-lookup"><span data-stu-id="91066-105">This one-way synchronization continues to run in the background to keep the Azure AD DS managed domain up-to-date with any changes from Azure AD.</span></span> <span data-ttu-id="91066-106">Azure AD DS 不会同步回 Azure AD。</span><span class="sxs-lookup"><span data-stu-id="91066-106">No synchronization occurs from Azure AD DS back to Azure AD.</span></span>

<span data-ttu-id="91066-107">有关 Azure Active Directory 域服务同步的更多详细信息，请参阅 [域服务同步](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization)。</span><span class="sxs-lookup"><span data-stu-id="91066-107">For more details on Azure Active Directory domain service synchronization, see [Domain Service Synchronization](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).</span></span> 
