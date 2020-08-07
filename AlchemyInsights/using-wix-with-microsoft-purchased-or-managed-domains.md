---
title: 将 Wix 网站与 Microsoft 购买或托管的域结合使用
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/05/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5855"
- "9003096"
ms.openlocfilehash: f6845c56f05e9cef11362ce601a974b73a154c9a
ms.sourcegitcommit: 28a319e482e6a8644e87726e1b0e599819df52d0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46572388"
---
# <a name="using-a-wix-website-with-microsoft-purchased-or-managed-domains"></a><span data-ttu-id="fd9af-102">将 Wix 网站与 Microsoft 购买或托管的域结合使用</span><span class="sxs-lookup"><span data-stu-id="fd9af-102">Using a Wix website with Microsoft purchased or managed domains</span></span>

<span data-ttu-id="fd9af-103">有关如何将 Wix 网站与 Microsoft 购买或托管的域结合使用的相关信息，请参阅[更新 DNS 记录，从而让网站继续使用当前托管提供商的服务](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)。</span><span class="sxs-lookup"><span data-stu-id="fd9af-103">For information about how to use a Wix website with a Microsoft purchased or managed domain, see [Update DNS records to keep your website with your current hosting provider](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider).</span></span>

<span data-ttu-id="fd9af-104">有关详细信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="fd9af-104">For details, see:</span></span> 

- <span data-ttu-id="fd9af-105">Wix 的文章《使用指针方法将域连接到 Wix》，建议添加上述链接中描述的 DNS 记录，而不是在使用 Microsoft 365 时更改名称服务器。</span><span class="sxs-lookup"><span data-stu-id="fd9af-105">The Wix article, "Connecting a Domain to Wix Using the Pointing Method," recommends adding DNS records as outlined in the link above rather than changing names servers when you're using Microsoft 365.</span></span>

- <span data-ttu-id="fd9af-106">如果你选择将名称服务器更改为 Wix，则必须在 Wix for Microsoft 处创建 DNS 记录。</span><span class="sxs-lookup"><span data-stu-id="fd9af-106">If you choose to change name servers to Wix, you must create DNS records at Wix for Microsoft.</span></span> <span data-ttu-id="fd9af-107">有关详细信息，请参阅[在 Wix for Microsoft 创建 DNS 记录](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix)。</span><span class="sxs-lookup"><span data-stu-id="fd9af-107">For more info, see [Create DNS records at Wix for Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix).</span></span>

- <span data-ttu-id="fd9af-108">如果您是从 Microsoft 购买的域名，则无法更改名称服务器。</span><span class="sxs-lookup"><span data-stu-id="fd9af-108">If your domain was purchased from Microsoft the name servers can't be changed.</span></span> <span data-ttu-id="fd9af-109">如果必须更改名称服务器，则必须在 60 天后将 Microsoft 购买的域迁移到另一个托管提供商。</span><span class="sxs-lookup"><span data-stu-id="fd9af-109">If you must change names servers, the Microsoft purchased domain must be transferred to another hosting provider after 60 days.</span></span> <span data-ttu-id="fd9af-110">有关详细信息，请参阅[域常见问题解答](https://docs.microsoft.com/microsoft-365/admin/setup/domains-faq#can-i-transfer-a-domain-i-purchased-from-microsoft-to-another-provider)。</span><span class="sxs-lookup"><span data-stu-id="fd9af-110">For more info, see the [Domains FAQ](https://docs.microsoft.com/microsoft-365/admin/setup/domains-faq#can-i-transfer-a-domain-i-purchased-from-microsoft-to-another-provider).</span></span>