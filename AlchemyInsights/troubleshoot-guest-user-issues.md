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
# <a name="troubleshoot-guest-user-issues"></a>来宾用户问题疑难解答

1. 有关管理对应用程序的来宾访问的指南，请参阅"使用 Azure AD 访问评审管理[来宾访问"。](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews)
1. 在[Azure](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal)门户中将来宾用户添加到你的目录：在此快速入门中，你将通过 Azure 门户将新的来宾用户添加到 Azure AD 目录，发送邀请，并查看来宾用户的邀请兑换过程。
1. [使用 PowerShell](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell)添加来宾用户：在此快速入门中，你将使用 New-AzureADMSInvitation 命令将一个来宾用户添加到 Azure 租户。
1. 若要了解如何从 Azure 门户中或通过使用 PowerShell 将用户和组分配给 Azure Active Directory (Azure AD) 中的企业应用程序，请参阅"在 [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal)中管理应用的用户分配"。 
1. Azure Active Directory (Azure AD) B2B 协作适用于与 Azure AD 集成大多数应用。 本文将 [介绍](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)配置一些热门 SaaS 应用以用于 Azure AD B2B 的说明。
1. 作为使用 Azure Active Directory (Azure AD) B2B 协作功能邀请合作伙伴组织的来宾用户加入 Azure AD 的组织，你现在可以提供这些 B2B 用户对本地应用的访问权限。 这些本地应用可以使用基于 SAML 的身份验证或集成 Windows 身份验证 (IWA) Kerberos 约束委派 (KCD) 。 有关详细信息，请参阅向 [Azure AD 中的 B2B 用户授予对本地应用程序的访问权限](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises)。
1. 了解如何使用 [Azure AD B2B](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)协作向本地托管的合作伙伴帐户授予对云资源的访问权限。