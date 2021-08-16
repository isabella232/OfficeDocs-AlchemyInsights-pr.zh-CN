---
title: 美国/英国护照号码的 DLP 规则不工作
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 85e3ed7fdc221981de13ab6e2ada8adf2a3a80b40ff163981e047cc4a02a1514
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004936"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>DLP 问题 - 美国/英国护照号码

**重要信息：** 在这段前所未有的时期，我们正在采取措施确保 SharePoint Online 和 OneDrive 服务高度可用，请访问 [SharePoint Online 临时功能调整](https://aka.ms/ODSPAdjustments)，获取详细信息。

**美国/英国护照号码的 DLP 问题**

在 O365 中使用 DLP 敏感信息类型时 (**DLP**) 数据丢失防护功能是否对包含美国 **/** 英国护照号的内容有效？ 如果是，请确保您的内容包含 DLP 策略在评估时查找的内容的所需信息。
  
例如，对于置信度为 75% 的美国 **/** 英国护照号码策略，将评估以下各项，并且必须检测到以下内容，规则触发
  
- **[格式：](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 九个数字

- **[模式：](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 九个连续的数字

- **[校验和：](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** 否，没有校验和

- **[定义：](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** DLP 策略 75% 确信在 300 个字符的邻近度内检测到这种类型的敏感信息：

  - 函数 Func_usa_uk_passport 找到与该模式匹配的内容。

  - 找到 Keyword_passport 中的一个关键字。

    例如，以下示例将触发美国 **/** 英国护照号码策略：美国护照号码123456789

有关内容需要检测美国/英国护照号码的内容详细信息，请参阅本文中的以下部分：敏感信息类型查找[美国/英国](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)护照号码的内容
  
使用不同的内置敏感信息类型，请参阅以下文章，了解其他类型的信息：敏感信息 [类型查找什么](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  