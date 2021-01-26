---
title: API 权限和同意
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/25/2021
ms.locfileid: "49951863"
---
# <a name="api-permissions-and-consent"></a><span data-ttu-id="d1363-102">API 权限和同意</span><span class="sxs-lookup"><span data-stu-id="d1363-102">API permissions and consent</span></span>

<span data-ttu-id="d1363-103">与 Microsoft 标识平台集成的应用程序遵循授权模型，使用户和管理员能够控制如何访问数据。</span><span class="sxs-lookup"><span data-stu-id="d1363-103">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="d1363-104">授权模型的实现已在 Microsoft 标识平台终结点上更新。</span><span class="sxs-lookup"><span data-stu-id="d1363-104">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint.</span></span> <span data-ttu-id="d1363-105">它更改应用必须与 Microsoft 标识平台交互的方式。</span><span class="sxs-lookup"><span data-stu-id="d1363-105">It changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="d1363-106">[Microsoft 标识平台终结点中](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 的权限和许可涵盖此授权模型的基本概念，包括范围、权限和同意。</span><span class="sxs-lookup"><span data-stu-id="d1363-106">[Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) covers the basic concepts of this authorization model, including scopes, permissions, and consent.</span></span>

<span data-ttu-id="d1363-107">Azure [Active Directory (Azure AD) 同意框架](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) 使开发多租户 Web 和本机客户端应用程序变得简单。</span><span class="sxs-lookup"><span data-stu-id="d1363-107">The [Azure Active Directory (Azure AD) consent framework](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) makes it easy to develop multi-tenant web and native client applications.</span></span> <span data-ttu-id="d1363-108">这些应用程序允许用户帐户从 Azure AD 租户登录，该租户不同于注册应用程序的租户。</span><span class="sxs-lookup"><span data-stu-id="d1363-108">These applications allow sign-in by user accounts from an Azure AD tenant that's different from the one where the application is registered.</span></span> <span data-ttu-id="d1363-109">除了你自己的 Web API 之外，他们还需要访问 Web API（如 Microsoft Graph API (）来访问 Microsoft 365) 和其他 Microsoft 服务 API 中的 Azure AD、Intune 和服务。</span><span class="sxs-lookup"><span data-stu-id="d1363-109">They may also need to access web APIs such as the Microsoft Graph API (to access Azure AD, Intune, and services in Microsoft 365) and other Microsoft services' APIs, in addition to your own web APIs.</span></span>

