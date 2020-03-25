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
ms.openlocfilehash: 6b28534d072c024a98a9b05f6cb55bfdc3435db6
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932433"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>包含信用卡号的 DLP 问题

**重要说明**：许多 SharePoint Online 和 OneDrive 客户对在后台运行的服务运行关键业务应用程序。 其中包括内容迁移、数据丢失防护（DLP）和备份解决方案。 在这些前所未有的时间内，我们将采取措施，以确保在远程工作方案中，SharePoint Online 和 OneDrive 服务对依赖于该服务的用户保持高可用性和可靠性。

为支持此目标，我们已在工作日白天营业时对后台应用（迁移、DLP 和备份解决方案）实施了更严格的限制限制。 在这些情况中，您应认为这些应用程序的吞吐量非常有限。 但是，在夜间和周末的时间内，服务将准备好处理来自后台应用程序的较大数量的请求。

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
  