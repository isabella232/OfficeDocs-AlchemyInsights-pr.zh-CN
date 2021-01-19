---
title: 用户同意疑难解答
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
- "7785"
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/18/2021
ms.locfileid: "49897701"
---
# <a name="troubleshoot-user-consent"></a><span data-ttu-id="2ea51-102">用户同意疑难解答</span><span class="sxs-lookup"><span data-stu-id="2ea51-102">Troubleshoot user consent</span></span>

1. <span data-ttu-id="2ea51-103">你可以配置最终用户如何通过 Azure 门户或 PowerShell 同意应用程序。</span><span class="sxs-lookup"><span data-stu-id="2ea51-103">You can configure how end-users consent to applications through the Azure Portal or PowerShell.</span></span> <span data-ttu-id="2ea51-104">有关详细信息 [，请参阅用户](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) 同意设置。</span><span class="sxs-lookup"><span data-stu-id="2ea51-104">See [User consent settings](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) for more information.</span></span>
1. <span data-ttu-id="2ea51-105">管理员还可使用 Microsoft [Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) 代表单个用户授予委派权限的许可。</span><span class="sxs-lookup"><span data-stu-id="2ea51-105">An administrator can also use the [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) to grant consent to delegated permissions on behalf of a single user.</span></span> <span data-ttu-id="2ea51-106">有关详细信息，请参阅"[代表用户获取访问权限"。](https://docs.microsoft.com/graph/auth-v2-user)</span><span class="sxs-lookup"><span data-stu-id="2ea51-106">For more information, see [Get access on behalf of a user](https://docs.microsoft.com/graph/auth-v2-user).</span></span>
1. <span data-ttu-id="2ea51-107">[用户同意错误](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)：本文讨论在同意应用程序的过程中可能会发生的错误。</span><span class="sxs-lookup"><span data-stu-id="2ea51-107">[User Consent Errors](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): this article discusses errors that can occur during the process of consenting to an application.</span></span> <span data-ttu-id="2ea51-108">如果要解决不包含任何错误消息的意外同意提示，请参阅 [Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)的身份验证方案。</span><span class="sxs-lookup"><span data-stu-id="2ea51-108">If you are troubleshooting unexpected consent prompts that do not contain any error messages, see [Authentication Scenarios for Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>