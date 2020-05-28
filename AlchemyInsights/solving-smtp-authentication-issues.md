---
title: 解决 SMTP 身份验证问题
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 814c49e8e65966a0c9f927b1f7bfb03d3dc3d637
ms.sourcegitcommit: 0e43e19448705f151846e9e9e1e0f47e12938fdf
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/15/2020
ms.locfileid: "44264333"
---
# <a name="solving-smtp-authentication-issues"></a>解决 SMTP 身份验证问题

如果在尝试发送 SMTP 电子邮件并通过客户端或应用程序进行身份验证时收到错误 5.7.57 或 5.7.3，则应检查以下内容：

- 在你的租户中或你尝试使用的邮箱中可能禁用了经过身份验证的 SMTP 提交（检查这两个设置）。 若要了解详细信息，请参阅[启用或禁用经过身份验证的客户端 SMTP 提交](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission)。

- 检查是否为租户启用了 [Azure 安全默认值](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)；如果已启用，则使用基本身份验证（也称为传统身份验证，该验证将使用用户名和密码）的 SMTP 身份验证将失败。
