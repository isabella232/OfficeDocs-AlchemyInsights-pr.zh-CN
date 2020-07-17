---
title: 使用 PowerShell 共享策略和组织关系
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 717cdd6827e243ac6bf375209a911937c97088d2
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2020
ms.locfileid: "44853979"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a><span data-ttu-id="0a126-102">使用 PowerShell 共享策略和组织关系</span><span class="sxs-lookup"><span data-stu-id="0a126-102">Use PowerShell for Sharing policies and Organization relationships</span></span>


<span data-ttu-id="0a126-103">对于组织关系，请查看以下对象的详细语法和参数信息：[Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation)、[New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship)、[Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) 和 [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship)。</span><span class="sxs-lookup"><span data-stu-id="0a126-103">For Organization relationships please review the detailed syntax and parameter information for : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  AND  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span></span>

<span data-ttu-id="0a126-104">若要创建共享策略，请使用 [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy)。</span><span class="sxs-lookup"><span data-stu-id="0a126-104">To create sharing policy use [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span></span> <span data-ttu-id="0a126-105">若要[将共享策略应用于邮箱或用户](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)，需要将 [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) 和 [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) 与新创建的策略结合使用。</span><span class="sxs-lookup"><span data-stu-id="0a126-105">To  [apply a sharing policy to a mailbox or user](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  you need to use a combination of  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) and [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) with the newly created policy.</span></span> <span data-ttu-id="0a126-106">若要[修改、禁用或移除共享策略](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)，需要使用 [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) 和 [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy)。</span><span class="sxs-lookup"><span data-stu-id="0a126-106">To  [modify, disable or remove a sharing policy](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  you need to use  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) and [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span></span>

<span data-ttu-id="0a126-107">**如需全面了解本主题，请阅读：**</span><span class="sxs-lookup"><span data-stu-id="0a126-107">**For full understanding of this topic please read:**</span></span>

[<span data-ttu-id="0a126-108">Exchange Online 中的共享</span><span class="sxs-lookup"><span data-stu-id="0a126-108">Sharing in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing)