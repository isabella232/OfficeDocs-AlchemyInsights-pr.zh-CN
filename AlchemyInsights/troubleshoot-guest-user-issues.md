---
title: 来宾用户问题疑难解答
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004358"
- "7822"
ms.openlocfilehash: 0f2a10b918fee067b167ab58ac2544a89e0c8ea1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/18/2021
ms.locfileid: "49897696"
---
# <a name="troubleshoot-guest-user-issues"></a><span data-ttu-id="f6efc-102">来宾用户问题疑难解答</span><span class="sxs-lookup"><span data-stu-id="f6efc-102">Troubleshoot guest user issues</span></span>

1. <span data-ttu-id="f6efc-103">有关管理对应用程序的来宾访问的指南，请参阅"使用 Azure AD 访问评审管理[来宾访问"。](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews)</span><span class="sxs-lookup"><span data-stu-id="f6efc-103">For guidance on managing guest access to applications, see [Manage guest access with Azure AD access reviews](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews).</span></span>
1. <span data-ttu-id="f6efc-104">在[Azure](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal)门户中将来宾用户添加到你的目录：在此快速入门中，你将通过 Azure 门户将新的来宾用户添加到 Azure AD 目录，发送邀请，并查看来宾用户的邀请兑换过程。</span><span class="sxs-lookup"><span data-stu-id="f6efc-104">[Add guest users to your directory in the Azure portal](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal): In this quickstart, you'll add a new guest user to your Azure AD directory via the Azure portal, send an invitation, and see what the guest user's invitation redemption process looks like.</span></span>
1. <span data-ttu-id="f6efc-105">[使用 PowerShell](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell)添加来宾用户：在此快速入门中，你将使用 New-AzureADMSInvitation 命令将一个来宾用户添加到 Azure 租户。</span><span class="sxs-lookup"><span data-stu-id="f6efc-105">[Add a guest user with PowerShell](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell): In this quickstart, you’ll use the New-AzureADMSInvitation command to add one guest user to your Azure tenant.</span></span>
1. <span data-ttu-id="f6efc-106">若要了解如何从 Azure 门户中或通过使用 PowerShell 将用户和组分配给 Azure Active Directory (Azure AD) 中的企业应用程序，请参阅"在 [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal)中管理应用的用户分配"。</span><span class="sxs-lookup"><span data-stu-id="f6efc-106">To learn how to assign users, and groups, to enterprise applications in Azure Active Directory (Azure AD), either from within the Azure portal or by using PowerShell, see [Manage user assignment for an app in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).</span></span> 
1. <span data-ttu-id="f6efc-107">Azure Active Directory (Azure AD) B2B 协作适用于与 Azure AD 集成大多数应用。</span><span class="sxs-lookup"><span data-stu-id="f6efc-107">Azure Active Directory (Azure AD) B2B collaboration works with most apps that integrate with Azure AD.</span></span> <span data-ttu-id="f6efc-108">本文将 [介绍](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)配置一些热门 SaaS 应用以用于 Azure AD B2B 的说明。</span><span class="sxs-lookup"><span data-stu-id="f6efc-108">In this [article](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps), we walk through instructions for configuring some popular SaaS apps for use with Azure AD B2B.</span></span>
1. <span data-ttu-id="f6efc-109">作为使用 Azure Active Directory (Azure AD) B2B 协作功能邀请合作伙伴组织的来宾用户加入 Azure AD 的组织，你现在可以提供这些 B2B 用户对本地应用的访问权限。</span><span class="sxs-lookup"><span data-stu-id="f6efc-109">As an organization that uses Azure Active Directory (Azure AD) B2B collaboration capabilities to invite guest users from partner organizations to your Azure AD, you can now provide these B2B users access to on-premises apps.</span></span> <span data-ttu-id="f6efc-110">这些本地应用可以使用基于 SAML 的身份验证或集成 Windows 身份验证 (IWA) Kerberos 约束委派 (KCD) 。</span><span class="sxs-lookup"><span data-stu-id="f6efc-110">These on-premises apps can use SAML-based authentication or Integrated Windows Authentication (IWA) with Kerberos constrained delegation (KCD).</span></span> <span data-ttu-id="f6efc-111">有关详细信息，请参阅向 [Azure AD 中的 B2B 用户授予对本地应用程序的访问权限](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises)。</span><span class="sxs-lookup"><span data-stu-id="f6efc-111">For more information, see [Grant B2B users in Azure AD access to your on-premises applications](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises).</span></span>
1. <span data-ttu-id="f6efc-112">了解如何使用 [Azure AD B2B](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)协作向本地托管的合作伙伴帐户授予对云资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="f6efc-112">Learn how to [grant locally-managed partner accounts access to cloud resources using Azure AD B2B collaboration](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud).</span></span>