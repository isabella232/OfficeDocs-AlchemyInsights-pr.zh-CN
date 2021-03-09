---
title: SSO 的无缝单一登录 (解决) 问题
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
ms.openlocfilehash: 507dc5a3bdc5f1bc27cf12865daf98df6c702827
ms.sourcegitcommit: f835aa80f2d85e9c0549be9395110377dba50f3d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2021
ms.locfileid: "50530815"
---
# <a name="troubleshoot-seamless-single-sign-on-sso-browser-issues"></a>SSO 的无缝单一登录 (解决) 问题

大多数用户都能够通过以下步骤解决其无缝 SSO 浏览器问题：

1. 确保浏览器是最新的。
2. 从浏览器中删除 Cookie 以删除无效的 SSO 会话，然后再次尝试登录。
3. 尝试使用其他浏览器登录。

**已知的浏览器问题**

- Firefox 上的无缝 SSO 在专用浏览模式下不起作用。
- 当启用增强保护模式时，Internet Explorer SSO 无法正常使用。
- 无缝 SSO 在 Microsoft Edge 上的专用浏览模式下 (旧版) 。
- 无缝 SSO 在 iOS 和 Android 上的移动浏览器上不起作用。

无缝 SSO 支持基于 Chromium 的下一版本的 Microsoft Edge，并且它按设计在 InPrivate 和来宾模式下工作。

**公告**

若要提出功能请求或询问有关无缝 SSO 的技术问题，请参阅 [Microsoft 问答&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html)
