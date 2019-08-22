---
title: 适用于美国银行帐户编号的 DLP 规则不起作用
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 0a32708b5ac8d95ec6777ada2d151a15f90d65bf
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529847"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>包含美国银行帐户号的 DLP 问题

在 O365 中使用 DLP 敏感信息类型时, 您是否遇到**数据丢失防护 (DLP)** 无法处理包含**美国银行帐号**的内容的问题？ 如果是这样, 请确保您的内容包含在评估时 DLP 策略要查找的内容所需的信息。
  
例如, 对于配置为可信度为 85% 的**美国银行帐户号**策略, 将对其进行评估, 并且必须检测到规则才能触发以下条件:
  
- **[格式:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 位

- **[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 连续数字。

- **[校验和:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** 否, 没有校验和

- **[定义:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** 如果 DLP 策略在300个字符的邻近度内检测到此类型的敏感信息, 则 DLP 策略 75% 确信它检测到这种类型的敏感信息:

  - 正则表达式 Regex_usa_bank_account_number 找到与该模式匹配的内容

  - 找到 Keyword_usa_Bank_Account 中的一个关键字。

    例如, 以下示例将触发**美国银行帐户号**策略: 检查帐户78344011

若要详细了解为你的内容检测**美国银行帐号**所需的内容, 请参阅本文中的以下部分:[这些敏感信息类型对美国银行帐号的外观](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
使用不同的内置敏感信息类型, 请参阅以下文章, 了解其他类型所需的信息:[敏感信息类型查找的内容](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  