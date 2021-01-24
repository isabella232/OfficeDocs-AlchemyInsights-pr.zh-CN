---
title: 用户预配的属性映射
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7851"
- "9004348"
ms.openlocfilehash: 8bbf554c533d960a304901d7cbb492b87e9bec71
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/22/2021
ms.locfileid: "49935339"
---
# <a name="user-provisioning-attribute-mapping"></a><span data-ttu-id="ed484-102">用户预配的属性映射</span><span class="sxs-lookup"><span data-stu-id="ed484-102">User-provisioning attribute mapping</span></span>

1. <span data-ttu-id="ed484-103">若要解决已知属性映射问题，请参阅 [属性映射](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings)。</span><span class="sxs-lookup"><span data-stu-id="ed484-103">To troubleshoot known attribute-mapping issues, see [Attribute mappings](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span></span> 
2. <span data-ttu-id="ed484-104">Microsoft Azure Active Directory (AD) 支持将用户预配到第三方 SaaS 应用程序，例如 Salesforce、G Suite 和其他应用程序。</span><span class="sxs-lookup"><span data-stu-id="ed484-104">Microsoft Azure Active Directory (AD) provides support for user provisioning to third-party SaaS applications such as Salesforce, G Suite and others.</span></span> <span data-ttu-id="ed484-105">如果为第三方 SaaS 应用程序启用了用户设置，则 Azure 门户通过属性映射控制其属性值。</span><span class="sxs-lookup"><span data-stu-id="ed484-105">If you enable user provisioning for a third-party SaaS application, the Azure portal controls its attribute values through attribute-mappings.</span></span> <span data-ttu-id="ed484-106">若要了解如何自定义默认属性映射，请参阅 [在 Azure Active Directory 中自定义 SaaS 应用程序的用户预配属性映射](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes)。</span><span class="sxs-lookup"><span data-stu-id="ed484-106">To learn how to customize the default attribute-mappings, see [Customize user provisioning attribute-mappings for SaaS applications in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span></span>
    - <span data-ttu-id="ed484-107">若要详细了解 SaaS 应用的用户设置，请参阅 [什么是 Azure AD 中自动 SaaS 应用用户设置？](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span><span class="sxs-lookup"><span data-stu-id="ed484-107">To learn more about SaaS app user provisioning, see [What is automated SaaS app user provisioning in Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span></span> 
3. <span data-ttu-id="ed484-108">为用户预配自定义属性映射时，可能会发现想要映射的属性不会显示在源属性列表中。</span><span class="sxs-lookup"><span data-stu-id="ed484-108">When customizing attribute-mappings for user provisioning, you might find that the attribute you want to map doesn't appear in the Source attribute list.</span></span> <span data-ttu-id="ed484-109">本文，即 [将属性从本地 Active Directory 同步到 Azure AD，以将其预配到应用程序](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping)，说明了如何通过将缺少的属性从本地 AD 同步到 Azure AD 来添加这一属性。</span><span class="sxs-lookup"><span data-stu-id="ed484-109">The [Sync an attribute from your on-premises Active Directory to Azure AD for provisioning to an application](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) article shows you how to add the missing attribute by synchronizing it from your on-premises AD to Azure AD.</span></span>
