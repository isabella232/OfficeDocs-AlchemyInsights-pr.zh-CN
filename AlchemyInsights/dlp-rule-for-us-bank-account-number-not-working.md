---
title: 美国银行帐号的 DLP 规则不工作
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: d19b2dcc29e23fab522159945496165338a117a47bfcfcadf0b93e4e5f14464f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005008"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>有关美国银行帐号的 DLP 问题

**重要信息：** 在这段前所未有的时期，我们正在采取措施确保 SharePoint Online 和 OneDrive 服务高度可用，请访问 [SharePoint Online 临时功能调整](https://aka.ms/ODSPAdjustments)，获取详细信息。

**有关美国银行帐号的 DLP 问题**

在 O365 中使用 DLP 敏感信息类型时 (**DLP**) 数据丢失防护功能是否无法用于包含美国银行帐号的内容？ 如果是，请确保您的内容包含 DLP 策略在评估时查找的内容的所需信息。
  
例如，对于置信水平为 85% 的 **"美国** 银行帐号"策略，将评估以下各项，并且必须检测到规则以触发：
  
- **[格式](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** ：8-17 个数字

- **[模式](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** ：8-17 个连续的数字。

- **[校验和：](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** 否，没有校验和

- **[定义：](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** DLP 策略 75% 确信在 300 个字符的邻近度内检测到这种类型的敏感信息：

  - 正则表达式Regex_usa_bank_account_number查找与模式匹配的内容

  - 找到 Keyword_usa_Bank_Account 中的一个关键字。

    例如，以下示例将针对 **美国** 银行帐号策略触发：Checking Account 78344011

有关内容需要检测 **美国** 银行帐号的信息，请参阅本文中的以下部分：敏感信息类型查找美国银行帐号 [的内容](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
使用不同的内置敏感信息类型，请参阅以下文章，了解其他类型的信息：敏感信息 [类型查找什么](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  