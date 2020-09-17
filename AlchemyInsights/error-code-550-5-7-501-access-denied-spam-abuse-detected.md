---
title: 错误代码 550 5.7.501 访问被拒绝，检测到垃圾邮件滥用
ms.author: chrisda
author: chrisda
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "351"
- "3100015"
ms.assetid: 3105905c-e7a0-42a7-9c5a-61dc56a1d6fc
ms.openlocfilehash: 6542450ca4d03daef4a7f63783d431d2091bc5e7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47784045"
---
# <a name="550-57501-access-denied-spam-abuse-detected"></a><span data-ttu-id="472c4-102">550 5.7.501 访问被拒绝，检测到的垃圾邮件滥用</span><span class="sxs-lookup"><span data-stu-id="472c4-102">550 5.7.501 Access denied, spam abuse detected</span></span>

<span data-ttu-id="472c4-103">通常，当用户使用分配给 Microsoft 365 中新租户的 *onmicrosoft.com* 域从 IP 地址发送电子邮件时，将会出现此消息。</span><span class="sxs-lookup"><span data-stu-id="472c4-103">Typically, this message occurs when users send email messages from IP addresses using the initial *.onmicrosoft.com* domain that's assigned to new tenants in Microsoft 365.</span></span> <span data-ttu-id="472c4-104">解决此问题最简单的方法是：</span><span class="sxs-lookup"><span data-stu-id="472c4-104">The easiest way to resolve this problem is to:</span></span>

1. <span data-ttu-id="472c4-105">[将域添加到你的租户](https://docs.microsoft.com/microsoft-365/admin/setup/add-domain)。</span><span class="sxs-lookup"><span data-stu-id="472c4-105">[Add a domain to your tenant](https://docs.microsoft.com/microsoft-365/admin/setup/add-domain).</span></span>

2. <span data-ttu-id="472c4-106">[将用户的主电子邮件地址更改](https://docs.microsoft.com/microsoft-365/admin/add-users/change-a-user-name-and-email-address) 为刚添加的新自定义域。</span><span class="sxs-lookup"><span data-stu-id="472c4-106">[Change your users' primary email address](https://docs.microsoft.com/microsoft-365/admin/add-users/change-a-user-name-and-email-address) to the new custom domain you just added.</span></span>
