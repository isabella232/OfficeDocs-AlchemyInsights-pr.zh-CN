---
title: 美国的 DLP 规则 / 英国护照号码不起作用
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 716d1030d93ce006c36d7925fb132e974ae8feb4
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2019
ms.locfileid: "28278060"
---
您有未正常运行的内容包含**数据丢失防护 (DLP)** 问题**美国 / 英国护照号码**时使用 O365 中的 DLP 敏感信息类型？如果是这样，确保您的内容包含所需的信息的 DLP 策略查找的内容时对它求值。 
  
例如，对于**美国 / 英国护照号码**配置的 75%的可信度级别的策略，以下计算和必须要触发的规则检测到 
  
- **[格式：](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 九个数字 
    
- **[模式：](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 九个连续的数字 
    
- **[校验和：](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** 否，没有无校验和 
    
- **[定义：](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** DLP 策略是相信它已检测到此类型的敏感信息的 75 %if、 内 300 个字符的邻近性： 
    
  - 函数 Func_usa_uk_passport 找到与该模式匹配的内容。
    
  - 找到 Keyword_passport 中的一个关键字。
    
    例如，下面的示例将触发的**美国 / 英国护照号码**策略： 美国护照号码 123456789 
    
上必需美国的详细信息 / 英国护照号码检测到了用于您的内容，请参阅本文中的以下部分：[什么敏感信息类型外观美国 / 英国护照号码](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
使用不同的内置敏感信息类型，请参阅以下文章，获取信息什么是需要其他类型：[查找什么敏感信息类型](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

