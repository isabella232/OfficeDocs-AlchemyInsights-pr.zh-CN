---
title: 对欺诈版检测检查安全提示进行故障排除
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.openlocfilehash: 98627edcd2b685673dda8a8a18821eddf9b64bc1
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2019
ms.locfileid: "32391199"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="6e598-102">对欺诈版检测检查安全提示进行故障排除</span><span class="sxs-lookup"><span data-stu-id="6e598-102">Troubleshooting the safety tip for fraud detection checks</span></span>



<span data-ttu-id="6e598-103">如果您正在获取安全提示, 显示 "发件人未通过我们的欺诈检测检查, 并且可能不是其显示为", 则发件人无法传递 DKIM 或 SPF 身份验证检查。</span><span class="sxs-lookup"><span data-stu-id="6e598-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="6e598-104">解决此问题的最佳方法是让发件人对自己进行授权。</span><span class="sxs-lookup"><span data-stu-id="6e598-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="6e598-105">如果发件人代表你发送, 则需要通过将发件人的 IP 地址添加到你的 SPF 记录来对其进行授权。</span><span class="sxs-lookup"><span data-stu-id="6e598-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="6e598-106">有关详细信息, 请参阅对[欺诈版检测的红色 (可疑) 安全提示进行故障排除检查](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/)。</span><span class="sxs-lookup"><span data-stu-id="6e598-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span> 
  
<span data-ttu-id="6e598-107">以下是一些可提供帮助的链接:</span><span class="sxs-lookup"><span data-stu-id="6e598-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="6e598-108">Office 365 如何使用发件人策略框架 (SPF) 来防止欺骗</span><span class="sxs-lookup"><span data-stu-id="6e598-108">How Office 365 uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)
    
- [<span data-ttu-id="6e598-109">在 Office 365 中设置 SPF 以防止欺骗</span><span class="sxs-lookup"><span data-stu-id="6e598-109">Set up SPF in Office 365 to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
    

