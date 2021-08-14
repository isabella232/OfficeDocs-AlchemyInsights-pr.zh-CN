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
ms.openlocfilehash: 08d3bfa84fd5ab31d7165090c392866d863898545ade7631e820a100eef89dea
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952563"
---
# <a name="admin-consent-issues"></a>管理员同意问题

1. 启用 [管理员同意工作流](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) ，以允许用户直接从许可屏幕请求管理员批准。

1. 如果你或应用程序的用户在同意过程中看到意外错误，请参阅本文中的疑难解答步骤：对应用程序执行同意时出现 [意外错误](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)。

1. 了解有关租户[管理员同意Microsoft 标识平台、](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)同意提示的工作原理以及如何评估租户范围内管理员[](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)[同意的请求。](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent)

1. 与应用程序集成Microsoft 标识平台遵循授权模型，使用户和管理员能够控制如何访问数据。 授权模型的实现已在 Microsoft 标识平台 终结点上更新，并且更改了应用必须与 Microsoft 标识平台 交互的方式。 有关[此授权模型（包括范围、权限和同意）的概述，](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent)请参阅 Microsoft 标识平台 终结点中的权限和许可。