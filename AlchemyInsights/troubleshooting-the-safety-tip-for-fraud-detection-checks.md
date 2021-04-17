---
title: 欺诈检测检查的安全提示疑难解答
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834721"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="18d62-102">欺诈检测检查的安全提示疑难解答</span><span class="sxs-lookup"><span data-stu-id="18d62-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="18d62-103">如果收到一条安全提示，提示"发件人未通过我们的欺诈检测检查，并且可能不是他们看起来的身份"，则发件人未能通过 DKIM 或 SPF 身份验证检查。</span><span class="sxs-lookup"><span data-stu-id="18d62-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="18d62-104">解决此问题的最佳方法是让发件人自行授权。</span><span class="sxs-lookup"><span data-stu-id="18d62-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="18d62-105">如果发件人代表你发送，则需要通过将发件人的 IP 地址添加到 SPF 记录来授权他们。</span><span class="sxs-lookup"><span data-stu-id="18d62-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="18d62-106">有关详细信息 [，请参阅针对欺诈 (检查) 红色和](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) 可疑邮件安全提示疑难解答。</span><span class="sxs-lookup"><span data-stu-id="18d62-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="18d62-107">下面是一些有助于以下功能的其他链接：</span><span class="sxs-lookup"><span data-stu-id="18d62-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="18d62-108">Microsoft 如何使用发件人策略框架 (SPF) 防止欺骗</span><span class="sxs-lookup"><span data-stu-id="18d62-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="18d62-109">设置 SPF 以防止欺骗</span><span class="sxs-lookup"><span data-stu-id="18d62-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
