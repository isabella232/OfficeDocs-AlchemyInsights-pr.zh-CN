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
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>欺诈检测检查的安全提示疑难解答

如果收到一条安全提示，提示"发件人未通过我们的欺诈检测检查，并且可能不是他们看起来的身份"，则发件人未能通过 DKIM 或 SPF 身份验证检查。 解决此问题的最佳方法是让发件人自行授权。 如果发件人代表你发送，则需要通过将发件人的 IP 地址添加到 SPF 记录来授权他们。
  
有关详细信息 [，请参阅针对欺诈 (检查) 红色和](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) 可疑邮件安全提示疑难解答。
  
下面是一些有助于以下功能的其他链接：
  
- [Microsoft 如何使用发件人策略框架 (SPF) 防止欺骗](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [设置 SPF 以防止欺骗](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
