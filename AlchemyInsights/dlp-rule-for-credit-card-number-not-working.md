---
title: 信用卡号的 DLP 规则不起作用
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 40a4a1668039b70455e09ee662359c05235645e8
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977188"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>包含信用卡号的 DLP 问题

**重要说明**：在这些前所未有的时间内，我们将采取措施来确保 sharepoint Online 和 OneDrive 服务保持高可用性-有关详细信息，请参阅[Sharepoint Online 临时功能调整](https://aka.ms/ODSPAdjustments)。

**包含信用卡号的 DLP 问题**

在 O365 中使用 DLP 敏感信息类型时，您是否遇到**数据丢失防护（DLP）** 无法处理包含**信用卡号**的内容的问题？ 如果是这样，请确保您的内容包含在评估时触发 DLP 策略所需的信息。 例如，对于配置为可信度为85% 的**信用卡策略**，将对以下项进行评估，并且必须检测到规则才能触发：
  
- **[格式：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 位数字，可以是格式化或无格式（dddddddddddddddd），并且必须通过 Luhn 测试。

- **[模式：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** 一种非常复杂且强大的模式，可检测到全球所有主要品牌的卡，包括签证、MasterCard、发现卡、JCB、美洲 Express、礼品卡和用餐卡。

- **[校验和：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** 是，Luhn 校验和

- **[定义：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** 如果 DLP 策略在300个字符的邻近度内检测到此类型的敏感信息，则 DLP 策略85% 确信它检测到这种类型的敏感信息：

  - 函数 Func_credit_card 找到与该模式匹配的内容。

  - 下列其中一项为真：

  - 找到 Keyword_cc_verification 中的一个关键字。

  - 找到 Keyword_cc_name 中的关键字

  - 函数 Func_expiration_date 找到正确日期格式的日期。

  - 校验和传递

    例如，以下示例将触发 DLP 信用卡号策略：

  - 签证： 4485 3647 3952 7352
  
  - 过期：2/2009

若要详细了解为您的内容检测**信用卡号**需要什么，请参阅本文中的以下部分：[有关信用卡号的敏感信息类型的外观](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
使用不同的内置敏感信息类型，请参阅以下文章，了解其他类型所需的信息：[敏感信息类型查找的内容](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  