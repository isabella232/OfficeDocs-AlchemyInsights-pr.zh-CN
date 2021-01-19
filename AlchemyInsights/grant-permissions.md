---
title: 授予权限
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
- "9004353"
- "7784"
ms.openlocfilehash: 9e686bd33414512b0a3a2bc24477832a508537a8
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/18/2021
ms.locfileid: "49897700"
---
# <a name="grant-permissions"></a><span data-ttu-id="ef205-102">授予权限</span><span class="sxs-lookup"><span data-stu-id="ef205-102">Grant permissions</span></span>

1. <span data-ttu-id="ef205-103">授予租户 **范围的** 管理员同意：请参阅向应用程序 [](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent)授予租户范围的管理员同意，获取有关从 Azure 门户、使用 Azure AD PowerShell 或同意提示本身授予租户范围的管理员同意的分步说明。</span><span class="sxs-lookup"><span data-stu-id="ef205-103">**Granting tenant-wide admin consent**: See [Grant tenant-wide admin consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) for step-by-step instructions for granting tenant-wide admin consent from the Azure portal, using Azure AD PowerShell, or from the consent prompt itself.</span></span>
1. <span data-ttu-id="ef205-104">代表特定用户授予 **同意：管理员** 还可使用 Microsoft [Graph API](https://docs.microsoft.com/graph/use-the-api)代表单个用户授予对委派权限的同意，而不是授予整个组织的同意。</span><span class="sxs-lookup"><span data-stu-id="ef205-104">**Granting consent on behalf of a specific user**: Instead of granting consent for the entire organization, an administrator can also use the [Microsoft Graph API](https://docs.microsoft.com/graph/use-the-api) to grant consent to delegated permissions on behalf of a single user.</span></span> <span data-ttu-id="ef205-105">有关详细信息，请参阅"[代表用户获取访问权限"。](https://docs.microsoft.com/graph/auth-v2-user)</span><span class="sxs-lookup"><span data-stu-id="ef205-105">For more information, see [Get access on behalf of a user](https://docs.microsoft.com/graph/auth-v2-user).</span></span>