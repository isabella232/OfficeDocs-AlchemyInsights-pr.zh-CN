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
ms.openlocfilehash: b138c05e87e70c18bb6528819a34f8a9501446d57dcf4dbac0734f70fbc3466b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999230"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>由于浏览器问题导致无法登录 Azure， (浏览器挂起、保持旋转、不加载等) 

中断可能会影响您。 请查看是否有正在进行的中断 [：Azure 运行状况状态](https://status.azure.com/status/history/)。

请注销所有活动的 Azure 会话。 启动 Web 浏览器的专用模式或隐身模式。

您还可以尝试刷新浏览器、使用另一个浏览器、删除缓存 Cookie（如果上述操作不起作用）。

了解更多信息： [解决登录问题](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**无法访问订阅**

在 [Azure 门户](https://portal.azure.com/)中，确保从右上方的帐户选择了正确的 Azure 目录。

在 [Azure 帐户中心](https://account.windowsazure.com/Subscriptions)中，确保所使用的帐户是帐户管理员。

了解更多信息： [未找到订阅疑难解答](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**无法访问计费历史记录**

帐户管理员需要确保访问帐单信息的用户作为来宾用户添加到 Azure Active Directory 中： [添加或删除新用户](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support)。

然后，需要向用户分配全局管理员角色： [向用户分配角色](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support)。

发布后，可以使用 RBAC 策略向用户授予计费访问权限： [授予对帐单的访问权限](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)。

**推荐文档**

-   [我无法登录来管理 Azure 订阅](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)