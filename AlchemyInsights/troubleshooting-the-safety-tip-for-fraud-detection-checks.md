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
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>对欺诈版检测检查安全提示进行故障排除



如果您正在获取安全提示, 显示 "发件人未通过我们的欺诈检测检查, 并且可能不是其显示为", 则发件人无法传递 DKIM 或 SPF 身份验证检查。 解决此问题的最佳方法是让发件人对自己进行授权。 如果发件人代表你发送, 则需要通过将发件人的 IP 地址添加到你的 SPF 记录来对其进行授权。
  
有关详细信息, 请参阅对[欺诈版检测的红色 (可疑) 安全提示进行故障排除检查](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/)。 
  
以下是一些可提供帮助的链接:
  
- [Office 365 如何使用发件人策略框架 (SPF) 来防止欺骗](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)
    
- [在 Office 365 中设置 SPF 以防止欺骗](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
    

