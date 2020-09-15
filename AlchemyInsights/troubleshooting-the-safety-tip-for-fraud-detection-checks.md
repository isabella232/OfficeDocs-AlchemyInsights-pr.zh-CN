---
title: 对欺诈版检测检查安全提示进行故障排除
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: e42b498070bf5d9bfc36110667da8cc0fd431524
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658400"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>对欺诈版检测检查安全提示进行故障排除

如果您正在获取安全提示，显示 "发件人未通过我们的欺诈检测检查，并且可能不是其显示为"，则发件人无法传递 DKIM 或 SPF 身份验证检查。 解决此问题的最佳方法是让发件人对自己进行授权。 如果发件人代表你发送，则需要通过将发件人的 IP 地址添加到你的 SPF 记录来对其进行授权。
  
有关详细信息，请参阅有关 [欺诈检测检查的红色 (可疑) 安全提示的疑难解答](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) 。
  
以下是一些可提供帮助的链接：
  
- [Microsoft 如何使用发件人策略框架 (SPF) 防止欺骗](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [设置 SPF 以帮助防止欺骗](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
