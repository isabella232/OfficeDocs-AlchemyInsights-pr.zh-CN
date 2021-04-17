---
title: 将 Wix 网站与 Office 365 购买或托管的域结合使用
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
- "9001516"
- "3582"
ms.openlocfilehash: ef2e7278b1a70aedca1b2ad9c13c249bf8b09c00
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825937"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a><span data-ttu-id="41956-102">将 Wix 网站与 Office 365 购买或托管的域结合使用</span><span class="sxs-lookup"><span data-stu-id="41956-102">Using Wix website with Office 365 purchased or managed domains</span></span>

- [<span data-ttu-id="41956-103">更新 DNS 记录以便利用当前的托管提供商继续托管网站</span><span class="sxs-lookup"><span data-stu-id="41956-103">Update DNS records to keep your website with your current hosting provider</span></span>](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- <span data-ttu-id="41956-104">Wix 的文章《使用指针方法将域连接到 Wix》建议始终指针（添加上述链接中的 DNS 记录），而不是在使用 Office 365 时更改名称服务器。</span><span class="sxs-lookup"><span data-stu-id="41956-104">Wix article "Connecting a Domain to Wix Using the Pointing Method" recommends using pointing (adding DNS records per the above link) rather than changing names servers when using Office 365</span></span>
- <span data-ttu-id="41956-105">如果你仍然选择将名称服务器更改为 Wix，则需要[在 Wix 处为 Microsoft 创建 DNS 记录](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)。</span><span class="sxs-lookup"><span data-stu-id="41956-105">If you still choose to change name servers to Wix you will then need to  [Create DNS records at Wix for Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)</span></span>
- <span data-ttu-id="41956-106">如果你的域是从 Microsoft 购买的，则无法更改名称服务器。</span><span class="sxs-lookup"><span data-stu-id="41956-106">If your domain was purchased from Microsoft the name servers cannot be changed.</span></span> <span data-ttu-id="41956-107">如果必须更改名称服务器，则必须[在 60 天后将从 Microsoft 购买的域迁移到另一个托管提供商](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)。</span><span class="sxs-lookup"><span data-stu-id="41956-107">If you have to change names servers the Microsoft purchased domain would need to be  [transferred to another hosting provider after 60 days](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)</span></span>