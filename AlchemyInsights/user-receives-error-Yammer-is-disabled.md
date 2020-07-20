---
title: 用户收到错误 AADSTS7000112 Yammer 被禁用
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2020
ms.locfileid: "45157274"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a>用户收到错误 AADSTS7000112 Yammer 被禁用

如果收到错误“ AADSTS7000112：应用程序'00000005-0000-0ff1-ce00-000000000000'（Yammer）被禁用”，则 Azure AD 中的服务主体存在问题。 管理员可能已禁用服务主体，阻止访问 Yammer。

建议不要禁用服务主体，否则会导致其他问题。 有关阻止用户访问 Yammer 的支持方法的详细信息，请参阅[关闭 Microsoft 365 用户访问 Yammer ](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access)。  

若要在 Azure 门户中更正此问题，并将用户访问权限还原到 Yammer：

1.  打开 “Azure Active Directory”页面，然后在左侧导航窗格的“**管理**”下选择“**企业应用程序**”。
3.  在搜索框中键入 **Office 365 Yammer **，然后选择应用程序名称以打开设置。
4.  在左侧导航窗格的“**管理**”下选择“**属性**”。
5.  将“**是否已启用供用户登录的值？**”设置为“**是**”，然后选择“**保存**”。
6.  重新登录 Yammer。 您可能需要清除 cookie。

或者运行 PowerShell 命令来设定数值。 有关更多信息，请参阅“[单击 Office 365 中的 Yammer 磁贴时，出现“抱歉，我们无法登录”错误](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365)”。 