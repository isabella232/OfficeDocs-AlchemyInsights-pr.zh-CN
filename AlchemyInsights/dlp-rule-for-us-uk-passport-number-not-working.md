---
title: 美国/英国护照号码的 DLP 规则不起作用
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 534e258c31a9a71c618765511487487c53f455b5
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977096"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>有关 DLP-美国/英国护照号码的问题

**重要说明**：在这些前所未有的时间内，我们将采取措施来确保 sharepoint Online 和 OneDrive 服务保持高可用性-有关详细信息，请参阅[Sharepoint Online 临时功能调整](https://aka.ms/ODSPAdjustments)。

**美国/英国护照号码的 DLP 问题**

在 O365 中使用 DLP 敏感信息类型时，您是否遇到**数据丢失防护（DLP）** 无法处理包含**美国/英国护照号码**的内容的问题？ 如果是这样，请确保您的内容包含在评估时 DLP 策略要查找的内容所需的信息。
  
例如，对于配置为可信度为75% 的**美国/英国护照号码**策略，将对以下项进行评估，并且必须检测到规则才能触发
  
- **[格式：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 九位数字

- **[模式：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 九个连续数字

- **[校验和：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** 否，没有校验和

- **[定义：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** 如果 DLP 策略在300个字符的邻近度内检测到此类型的敏感信息，则 DLP 策略75% 确信它检测到这种类型的敏感信息：

  - 函数 Func_usa_uk_passport 找到与该模式匹配的内容。

  - 找到 Keyword_passport 中的一个关键字。

    例如，以下示例将触发**美国/英国护照号码**策略：美国护照号码123456789

若要详细了解为你的内容检测美国/英国护照号码时所需的信息，请参阅本文中的以下部分：[敏感信息类型查找美国/英国护照号码的内容](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
使用不同的内置敏感信息类型，请参阅以下文章，了解其他类型所需的信息：[敏感信息类型查找的内容](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  