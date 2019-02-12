---
title: DLP 规则 SSN 不起作用
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: d2d21fb5546d36990d69b76e3ceb72ce2edf3d80
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/12/2019
ms.locfileid: "29933470"
---
您是否有问题**数据丢失防护 (DLP)** 包含**社会保险号码 (SSN)** 时使用 Office 365 中的敏感信息类型的内容不起作用？如果是这样，请确保您的内容包含的 DLP 策略正在查找所需的信息。 
  
例如，对于配置了 85%可信度 SSN 策略，以下计算和必须要触发的规则检测到：
  
- **[格式：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 位，可能会在带格式或无格式的模式 
    
- **[模式：](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** 四个函数在四个不同的模式中查找 Ssn: 
    
  - Func_ssn 查找具有 2011 年以前使用短划线或空格格式化的强格式的 SSN（ddd-dd-dddd 或 ddd dd dddd）
    
  - Func_unformatted_ssn 查找具有 2011 年以前未格式化为 9 个连续数字的强格式的 SSN (ddddddddd)
    
  - Func_randomized_formatted_ssn 查找 2011 年后使用短划线或空格（ddd-dd-dddd 或 ddd dd dddd）格式化的 SSN
    
  - Func_randomized_unformatted_ssn 查找 2011 年后未格式化为 9 个连续数字 (ddddddddd) 的 SSN
    
- **[校验和：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** 否，没有无校验和 
    
- **[定义：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** DLP 策略是 85%相信它已检测到此类型的敏感信息 if、 内 300 个字符的邻近性： 
    
  - [函数 Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)查找与模式匹配的内容。 
    
  - 找到从[Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn)关键字。关键字的示例包括：*社会保险社会保险 #、 Soc 秒、 SSN* 。例如，下面的示例将触发 DLP SSN 策略： **SSN: 489-36 8350**
    
什么是需要 Ssn 检测到了用于您的内容的详细信息，请参阅本文中的以下部分：[什么敏感信息类型查找 Ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
使用不同的内置敏感信息类型，请参阅以下文章，获取信息什么是需要其他类型：[查找什么敏感信息类型](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

