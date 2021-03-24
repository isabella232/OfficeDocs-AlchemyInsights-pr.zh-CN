---
title: 应用注册客户端密码或证书问题
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9685"
ms.openlocfilehash: 990648d286ec801785201e6513b70534c3d80e3f
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123065"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a><span data-ttu-id="d1bef-102">应用注册客户端密码或证书问题</span><span class="sxs-lookup"><span data-stu-id="d1bef-102">App Registration client secret or Certificate issues</span></span>

<span data-ttu-id="d1bef-103">应用程序客户端密码是否即将过期？</span><span class="sxs-lookup"><span data-stu-id="d1bef-103">Application client secret expiring?</span></span>

<span data-ttu-id="d1bef-104">无论是通过应用注册门户中的标准注册过程，还是使用应用程序许可在租户中创建服务主体，都需要在当前客户端密码过期之前创建一个新的客户端密码，并更新相关应用程序代码。</span><span class="sxs-lookup"><span data-stu-id="d1bef-104">Regardless of how the registered application was created, whether through the standard registration process in the Apps Registration portal or if the Service Principal was created in your tenant using application consent, a new Client Secret will need to be created prior to the expiration of the current one and updated in the related application code.</span></span> <span data-ttu-id="d1bef-105">最长有效期为 2 年。</span><span class="sxs-lookup"><span data-stu-id="d1bef-105">The maximum validity period is 2 years.</span></span> <span data-ttu-id="d1bef-106">提醒一下，必须记录密码值，因为它在门户中离开应用注册页面后将不再可见。</span><span class="sxs-lookup"><span data-stu-id="d1bef-106">As a reminder the secret value must be recorded as it will no longer be visible after leaving the App registrations page in the portal.</span></span> <span data-ttu-id="d1bef-107">有关详细信息，请参阅 [快速入门：在 Microsoft](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) 标识平台中注册应用和 [Microsoft 标识平台最佳做法](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)。</span><span class="sxs-lookup"><span data-stu-id="d1bef-107">For more information, see [Quickstart: Register an app in the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) and [Best practices for the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).</span></span>

<span data-ttu-id="d1bef-108">若要了解更多信息，请参阅在门户 - Microsoft 标识平台 & Azure [AD](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)应用和服务主体。</span><span class="sxs-lookup"><span data-stu-id="d1bef-108">To learn more, see [Create an Azure AD app & service principal in the portal - Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).</span></span>
