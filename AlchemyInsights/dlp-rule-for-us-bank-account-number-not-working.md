---
title: 美国银行帐号不起作用的 DLP 规则
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 6eae9146d33f5fc307085dbf931d57bdbb28b82e
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29459074"
---
您是否有问题**数据丢失防护 (DLP)** 包含**美国银行帐号**O365 中使用的 DLP 敏感信息类型时的内容不起作用？如果是这样，确保您的内容包含所需的信息的 DLP 策略查找的内容时对它求值。 
  
例如，**美国银行帐号**策略配置了 85%可信度，以下计算和必须要触发的规则检测到： 
  
- **[格式：](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8 17 数字 
    
- **[模式：](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8 17 连续的数字。 
    
- **[校验和：](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** 否，没有无校验和 
    
- **[定义：](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)** DLP 策略是相信它已检测到此类型的敏感信息的 75 %if、 内 300 个字符的邻近性： 
    
  - 正则表达式 Regex_usa_bank_account_number 找到与该模式匹配的内容。
    
  - 找到 Keyword_usa_Bank_Account 中的一个关键字。
    
    例如，下面的示例将触发**美国银行帐号**策略： 检查帐户 78344011 
    
什么是**美国银行帐号**检测到了用于您的内容所需的详细信息，请参阅本文中的以下部分：[什么敏感信息类型查找美国银行帐号](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
使用不同的内置敏感信息类型，请参阅以下文章，获取信息什么是需要其他类型：[查找什么敏感信息类型](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

