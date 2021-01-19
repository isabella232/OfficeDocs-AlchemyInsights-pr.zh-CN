---
title: 管理员同意问题
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
- "9004354"
- "7786"
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/18/2021
ms.locfileid: "49888292"
---
# <a name="admin-consent-issues"></a><span data-ttu-id="33c80-102">管理员同意问题</span><span class="sxs-lookup"><span data-stu-id="33c80-102">Admin consent issues</span></span>

1. <span data-ttu-id="33c80-103">启用 [管理员同意工作流](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) ，以允许用户直接从同意屏幕请求管理员批准。</span><span class="sxs-lookup"><span data-stu-id="33c80-103">Enable the [admin consent workflow](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) to allow users to request administrator approval directly from the consent screen.</span></span>

1. <span data-ttu-id="33c80-104">如果你或应用程序的用户在同意过程中看到意外错误，请参阅本文了解疑难解答步骤：对应用程序执行同意时出现意外 [错误](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)。</span><span class="sxs-lookup"><span data-stu-id="33c80-104">If you or your application's users are seeing unexpected errors during the consent process, see this article for troubleshooting steps: [Unexpected error when performing consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>

1. <span data-ttu-id="33c80-105">了解有关 Microsoft[标识](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)平台上的管理员同意、同意提示的工作原理[](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)以及如何评估租户范围内管理员同意[的请求等内容。](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent)</span><span class="sxs-lookup"><span data-stu-id="33c80-105">Learn more about [Admin consent on the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), how the [consent prompt](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) works, and how to [evaluate a request for tenant-wide admin consent](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span></span>

1. <span data-ttu-id="33c80-106">与 Microsoft 标识平台集成的应用程序遵循授权模型，使用户和管理员能够控制如何访问数据。</span><span class="sxs-lookup"><span data-stu-id="33c80-106">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="33c80-107">授权模型的实现已在 Microsoft 标识平台终结点上更新，它更改了应用必须与 Microsoft 标识平台交互的方式。</span><span class="sxs-lookup"><span data-stu-id="33c80-107">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint, and it changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="33c80-108">有关 [此授权模型（](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) 包括范围、权限和同意）的概述，请参阅 Microsoft 标识平台终结点中的权限和许可。</span><span class="sxs-lookup"><span data-stu-id="33c80-108">See [Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) for an overview of this authorization model, including scopes, permissions, and consent.</span></span>