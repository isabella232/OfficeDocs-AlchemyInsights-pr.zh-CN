---
title: 订阅访问
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/27/2020
ms.locfileid: "48773769"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>由于浏览器问题 (浏览器挂起、保持旋转、不会加载等等，因此无法登录 Azure ) 

中断可能会受到影响。 请查看是否存在正在进行的中断： [Azure 运行状况状态](https://status.azure.com/status/history/)。

请注销所有活动的 Azure 会话。 启动 web 浏览器的私有或 incognito 模式。

您还可以尝试刷新浏览器，使用另一个浏览器，如果上面不起作用，则删除缓存 cookie。

了解详细信息： [解决登录问题](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**无法访问订阅**

在 [Azure 门户](https://portal.azure.com/)中，请确保从右上角的帐户中选择了正确的 Azure 目录。

在 [Azure 帐户中心](https://account.windowsazure.com/Subscriptions)中，确保使用的帐户是帐户管理员。

了解详细信息： [排除未找到订阅的故障](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**无法访问帐单历史记录**

帐户管理员需要确保以来宾用户身份在 Azure Active directory 中添加访问帐单信息的用户： [添加或删除新用户](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support)。

然后，需要向用户授予全局管理员角色：为 [用户分配角色](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support)。

发布此内容时，可以使用 RBAC 策略对用户授予帐单访问权限： [授予对帐单的访问权限](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)。

**建议的文档**

-   [我无法登录以管理我的 Azure 订阅](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)