---
title: 欺诈检测安全提示疑难解答
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
ms.openlocfilehash: c7ee1fcc887a3221b5f2acda1aa6ae6beb03cb96686d4ecb7828a02f8ff48302
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955956"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>欺诈检测安全提示疑难解答

如果你收到一安全提示"发件人未通过我们的欺诈检测检查，并且可能不是他们看起来的身份"，则发件人未能通过 DKIM 或 SPF 身份验证检查。 解决此问题的最佳方法是让发件人自行授权。 如果发件人代表你发送，则需要通过将发件人的 IP 地址添加到 SPF 记录来授权他们。
  
有关详细信息[，请参阅解决 (可疑) 安全提示欺诈检测检查](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/)问题。
  
下面是一些有助于以下功能的其他链接：
  
- [Microsoft 如何使用发件人策略框架 (SPF) 防止欺骗](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [设置 SPF 以防止欺骗](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
