---
title: 准备好在 Microsoft 365 中使用 TLS 1.2
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Critical
ms.custom:
- "1266"
- "1600052"
ms.assetid: d5c84f5c-a3ca-4abd-8633-7e9ff01328a9
ms.openlocfilehash: 1ec40ba36c69296298e24dca64a873d53682833a
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085894"
---
# <a name="prepare-for-use-of-tls-12-in-microsoft-365"></a><span data-ttu-id="86439-102">准备好在 Microsoft 365 中使用 TLS 1.2</span><span class="sxs-lookup"><span data-stu-id="86439-102">Prepare for use of TLS 1.2 in Microsoft 365</span></span>

<span data-ttu-id="86439-103">自 2018 年 10 月 31 日起，Microsoft 365 将继续向 TLS 1.2 过渡。</span><span class="sxs-lookup"><span data-stu-id="86439-103">As of October 31st, 2018, Microsoft 365 will continue transitioning to TLS 1.2.</span></span> <span data-ttu-id="86439-104">自 2020 年 10 月 15 日起，O365 将开始在服务中弃用 TLS 1.0 和 1.1。</span><span class="sxs-lookup"><span data-stu-id="86439-104">Starting October 15, 2020, O365 will begin the deprecation of TLS 1.0 and 1.1 across the service.</span></span> <span data-ttu-id="86439-105">此更改的推出将在未来几个星期和几个月内继续进行，但客户应假定自 2020 年 10 月 15 日起、与 O365 交互时， TLS 1.0/1.1 调用不工作。</span><span class="sxs-lookup"><span data-stu-id="86439-105">The rollout of this change will continue over the next few weeks and months, but customers should assume no TLS 1.0/1.1 calls will work when engaging with O365 starting Oct 15, 2020.</span></span> <span data-ttu-id="86439-106">如前所述（2017 年 12 月的 MC126199、2018 年 2 月的 MC128929、2019 年 7 月的 MC186827 和 2020 年 7 月的 MC218794），我们正将所有在线服务转到传输层安全性 (TLS) 1.2+，以在默认情况下、提供最佳加密并提高服务安全性。</span><span class="sxs-lookup"><span data-stu-id="86439-106">As previously communicated (MC126199 in Dec 2017, MC128929 in Feb 2018, MC186827 in July 2019, and MC218794 in July 2020), we are moving all of our online services to Transport Layer Security (TLS) 1.2+ to provide best-in-class encryption, and to ensure our service is more secure, by default.</span></span> <span data-ttu-id="86439-107">客户仍可选择在其服务器和资源上使用 TLS 1.0/1.1，但他们应假定与 O365 资源交互时，只有 TLS 1.2 或更高版本工作。</span><span class="sxs-lookup"><span data-stu-id="86439-107">Customers can still choose to have TLS 1.0/1.1 on their servers and resources, but they should assume only TLS 1.2 or higher will work when interacting with O365 resources.</span></span>
  
<span data-ttu-id="86439-108">若要了解有关这些更改的详细信息，请参阅 [此处](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide) 和 [此处](https://docs.microsoft.com/microsoft-365/compliance/tls-1.0-and-1.1-deprecation-for-office-365?view=o365-worldwide)。</span><span class="sxs-lookup"><span data-stu-id="86439-108">To learn more about these changes, please see [here](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide) and [here](https://docs.microsoft.com/microsoft-365/compliance/tls-1.0-and-1.1-deprecation-for-office-365?view=o365-worldwide).</span></span>

  