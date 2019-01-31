---
title: 疑难解答欺诈检测安全提示检查
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.openlocfilehash: 06a0b5b8d29052e6033de5938b8ea67ceabc9848
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29658105"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="205c6-102">疑难解答欺诈检测安全提示检查</span><span class="sxs-lookup"><span data-stu-id="205c6-102">Troubleshooting the safety tip for fraud detection checks</span></span>



<span data-ttu-id="205c6-p101">如果您是获取安全提示的说"发件人我们欺诈检测检查失败，可能无法在谁它们显示为"，然后发件人无法通过 DKIM 或 SPF 身份验证检查。要解决此问题的最佳方法是发件人授权本身。如果发件人发送替您，您需要通过将发件人的 IP 地址添加到您的 SPF 记录授权他们。</span><span class="sxs-lookup"><span data-stu-id="205c6-p101">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks. The best method to resolve this is for the sender to authorize themselves. If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="205c6-106">有关详细信息，请参阅[疑难解答欺诈检测红色 （可疑） 安全提示检查](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/)。</span><span class="sxs-lookup"><span data-stu-id="205c6-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span> 
  
<span data-ttu-id="205c6-107">下面是一些可帮助的其他链接：</span><span class="sxs-lookup"><span data-stu-id="205c6-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="205c6-108">Office 365 如何使用发件人策略框架 (SPF) 来防止欺骗</span><span class="sxs-lookup"><span data-stu-id="205c6-108">How Office 365 uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)
    
- [<span data-ttu-id="205c6-109">在 Office 365 中设置 SPF 以防止欺骗</span><span class="sxs-lookup"><span data-stu-id="205c6-109">Set up SPF in Office 365 to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
    

