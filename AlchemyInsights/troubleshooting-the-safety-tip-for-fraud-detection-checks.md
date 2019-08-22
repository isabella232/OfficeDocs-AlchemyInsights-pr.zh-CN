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
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 7ce8bcc7caefebf51fc8d9622367fd16405deef1
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36533151"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="78ef6-102">对欺诈版检测检查安全提示进行故障排除</span><span class="sxs-lookup"><span data-stu-id="78ef6-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="78ef6-103">如果您正在获取安全提示, 显示 "发件人未通过我们的欺诈检测检查, 并且可能不是其显示为", 则发件人无法传递 DKIM 或 SPF 身份验证检查。</span><span class="sxs-lookup"><span data-stu-id="78ef6-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="78ef6-104">解决此问题的最佳方法是让发件人对自己进行授权。</span><span class="sxs-lookup"><span data-stu-id="78ef6-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="78ef6-105">如果发件人代表你发送, 则需要通过将发件人的 IP 地址添加到你的 SPF 记录来对其进行授权。</span><span class="sxs-lookup"><span data-stu-id="78ef6-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="78ef6-106">有关详细信息, 请参阅对[欺诈版检测的红色 (可疑) 安全提示进行故障排除检查](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/)。</span><span class="sxs-lookup"><span data-stu-id="78ef6-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="78ef6-107">以下是一些可提供帮助的链接:</span><span class="sxs-lookup"><span data-stu-id="78ef6-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="78ef6-108">Office 365 如何使用发件人策略框架 (SPF) 来防止欺骗</span><span class="sxs-lookup"><span data-stu-id="78ef6-108">How Office 365 uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="78ef6-109">在 Office 365 中设置 SPF 以防止欺骗</span><span class="sxs-lookup"><span data-stu-id="78ef6-109">Set up SPF in Office 365 to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
