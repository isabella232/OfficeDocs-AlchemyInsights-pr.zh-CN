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
# <a name="admin-consent-issues"></a>管理员同意问题

1. 启用 [管理员同意工作流](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) ，以允许用户直接从同意屏幕请求管理员批准。

1. 如果你或应用程序的用户在同意过程中看到意外错误，请参阅本文了解疑难解答步骤：对应用程序执行同意时出现意外 [错误](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)。

1. 了解有关 Microsoft[标识](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)平台上的管理员同意、同意提示的工作原理[](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)以及如何评估租户范围内管理员同意[的请求等内容。](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent)

1. 与 Microsoft 标识平台集成的应用程序遵循授权模型，使用户和管理员能够控制如何访问数据。 授权模型的实现已在 Microsoft 标识平台终结点上更新，它更改了应用必须与 Microsoft 标识平台交互的方式。 有关 [此授权模型（](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) 包括范围、权限和同意）的概述，请参阅 Microsoft 标识平台终结点中的权限和许可。