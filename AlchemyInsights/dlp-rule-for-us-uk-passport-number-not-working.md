---
title: 美国的 DLP 规则 / 英国护照号码不起作用
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: bb80ef07364a575f6032bb105cff83cd8f95bd63
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/12/2019
ms.locfileid: "29912086"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>问题 DLP-美国 / 英国护照号码

您有未正常运行的内容包含**数据丢失防护 (DLP)** 问题**美国 / 英国护照号码**时使用 O365 中的 DLP 敏感信息类型？如果是这样，确保您的内容包含所需的信息的 DLP 策略查找的内容时对它求值。 
  
例如，对于**美国 / 英国护照号码**配置的 75%的可信度级别的策略，以下计算和必须要触发的规则检测到 
  
- **[格式：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 九个数字 
    
- **[模式：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 九个连续的数字 
    
- **[校验和：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** 否，没有无校验和 
    
- **[定义：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** DLP 策略是相信它已检测到此类型的敏感信息的 75 %if、 内 300 个字符的邻近性： 
    
  - 函数 Func_usa_uk_passport 找到与该模式匹配的内容。
    
  - 找到 Keyword_passport 中的一个关键字。
    
    例如，下面的示例将触发的**美国 / 英国护照号码**策略： 美国护照号码 123456789 
    
上必需美国的详细信息 / 英国护照号码检测到了用于您的内容，请参阅本文中的以下部分：[什么敏感信息类型外观美国 / 英国护照号码](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
使用不同的内置敏感信息类型，请参阅以下文章，获取信息什么是需要其他类型：[查找什么敏感信息类型](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

