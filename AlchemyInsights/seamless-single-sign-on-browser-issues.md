---
title: 解决 SSO 的无缝单一 (登录) 浏览器问题
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
- "9004357"
- "9377"
ms.openlocfilehash: f8617c15072f70778f7f4b151e75ffce4749f89ffa2b4d91730937c26aaeabbb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074274"
---
# <a name="troubleshoot-seamless-single-sign-on-sso-browser-issues"></a>解决 SSO 的无缝单一 (登录) 浏览器问题

大多数用户可以使用以下步骤解决其无缝 SSO 浏览器问题：

1. 确保浏览器是最新的。
2. 从浏览器中删除 Cookie 以删除无效的 SSO 会话，然后再次尝试登录。
3. 请尝试使用不同的浏览器登录。

**已知浏览器问题**

- 无缝 SSO 在 Firefox 上的专用浏览模式下不起作用。
- 当增强保护模式打开时，Internet Explorer SSO 无法正常使用。
- 在旧版应用上，无缝 SSO 在专用Microsoft Edge (模式下) 。
- 无缝 SSO 在 iOS 和 Android 上的移动浏览器中不起作用。

无缝 SSO 支持下一版本的Microsoft Edge基于Chromium并且它按设计在 InPrivate 和来宾模式下工作。

**公告**

若要就无缝 SSO 提出功能请求或提出技术问题，请参阅 [Microsoft 问答&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html)
