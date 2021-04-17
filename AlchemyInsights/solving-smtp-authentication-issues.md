---
title: 解决 SMTP 身份验证问题
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 2d3f0f6b700c3e4485c9064fbaa4bcc165e92e17
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826405"
---
# <a name="solving-smtp-authentication-issues"></a><span data-ttu-id="5adaa-102">解决 SMTP 身份验证问题</span><span class="sxs-lookup"><span data-stu-id="5adaa-102">Solving SMTP authentication issues</span></span>

<span data-ttu-id="5adaa-103">如果在尝试发送 SMTP 电子邮件并通过客户端或应用程序进行身份验证时收到错误 5.7.57 或 5.7.3，则应检查以下内容：</span><span class="sxs-lookup"><span data-stu-id="5adaa-103">If you are getting errors 5.7.57 or 5.7.3 when trying to send SMTP email and authenticate with a client or application, there are a few things you should check:</span></span>

- <span data-ttu-id="5adaa-104">在你的租户中或你尝试使用的邮箱中可能禁用了经过身份验证的 SMTP 提交（检查这两个设置）。</span><span class="sxs-lookup"><span data-stu-id="5adaa-104">Authenticated SMTP submission might be disabled in your tenant, or on the mailbox that you are trying to use (check both settings).</span></span> <span data-ttu-id="5adaa-105">若要了解详细信息，请参阅[启用或禁用经过身份验证的客户端 SMTP 提交](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission)。</span><span class="sxs-lookup"><span data-stu-id="5adaa-105">To read more, see [Enable or disable authenticated client SMTP submission](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span></span>

- <span data-ttu-id="5adaa-106">检查是否为租户启用了 [Azure 安全默认值](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)；如果已启用，则使用基本身份验证（也称为传统身份验证，该验证将使用用户名和密码）的 SMTP 身份验证将失败。</span><span class="sxs-lookup"><span data-stu-id="5adaa-106">Check whether [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) are enabled for your tenant; if enabled, SMTP authentication using basic authentication (also known as legacy; this will use username and password) will fail.</span></span>
