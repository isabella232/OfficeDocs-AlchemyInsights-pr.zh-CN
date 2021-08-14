---
title: 信用卡号的 DLP 规则不工作
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
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: bd4f200233d5571fc7b01576038e7b3951a07716a7d5948005418d2896291ee5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005080"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>信用卡号的 DLP 问题

**重要信息：** 在这段前所未有的时期，我们正在采取措施确保 SharePoint Online 和 OneDrive 服务高度可用，请访问 [SharePoint Online 临时功能调整](https://aka.ms/ODSPAdjustments)，获取详细信息。

**信用卡号的 DLP 问题**

在 O365 中使用 DLP 敏感信息类型时 (**DLP**) 无法处理包含信用卡号的内容时，您是否遇到数据丢失防护问题？ 如果是，请确保内容中包含在评估 DLP 策略时触发该策略所需的信息。 例如，对于置信度为 85% 的信用卡策略，将评估以下各项，并且必须检测到规则以触发：
  
- **[](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 格式：16 个数字，可以格式化或无格式 (ddddddd) ) 必须通过 Luhn 测试。

- **[模式：](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** 非常复杂且强大的模式，可检测来自全球所有主要品牌的卡，包括 Visa、MasterCard、Discover Card、JCB、American Express、名片和第三者卡。

- **[校验和：](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** 是，Luhn 校验和

- **[定义：](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** 如果在 300 个字符的邻近度内，DLP 策略 85% 确信它检测到这种类型的敏感信息：

  - 函数 Func_credit_card 找到与该模式匹配的内容。

  - 下列其中一项为真：

  - 找到 Keyword_cc_verification 中的一个关键字。

  - 找到来自Keyword_cc_name的关键字

  - 函数 Func_expiration_date 找到正确日期格式的日期。

  - 校验和传递

    例如，以下示例将触发 DLP 信用卡号策略：

  - Visa：4485 3647 3952 7352
  
  - 过期时间：2009 年 2 月

有关内容需要检测信用卡号的内容详细信息，请参阅本文中的以下部分：敏感信息类型查找[信用卡的内容#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
使用不同的内置敏感信息类型，请参阅以下文章，了解其他类型的信息：敏感信息 [类型查找什么](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  