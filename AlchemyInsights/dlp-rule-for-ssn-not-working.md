---
title: SSN 的 DLP 规则不工作
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
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 3f30998fb3bc4c5442e4e1541b87d88ecd7df6eef3a50e719fa5014eb86af39c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004972"
---
# <a name="dlp-issues-with-social-security-numbers"></a>社会安全号码的 DLP 问题

**重要信息：** 在这段前所未有的时期，我们正在采取措施确保 SharePoint Online 和 OneDrive 服务高度可用，请访问 [SharePoint Online 临时功能调整](https://aka.ms/ODSPAdjustments)，获取详细信息。

**SSN 的 DLP 问题**

在使用 (中的敏感信息类型时，您是否遇到数据丢失防护 **) DLP** (**SSN**) 的内容无法Microsoft 365？ 如果是，请确保您的内容包含 DLP 策略所查找内容所需的信息。 
  
例如，对于置信度为 85% 的 SSN 策略，将评估以下各项，并且必须检测到规则以触发：
  
- **[格式：9](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 个数字，可能采用格式化或无格式模式

- **[模式：](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** 四个函数以四种不同的模式查找 SSN：

  - Func_ssn 查找具有 2011 年以前使用短划线或空格格式化的强格式的 SSN（ddd-dd-dddd 或 ddd dd dddd）

  - Func_unformatted_ssn 查找具有 2011 年以前未格式化为 9 个连续数字的强格式的 SSN (ddddddddd)

  - Func_randomized_formatted_ssn 查找 2011 年后使用短划线或空格（ddd-dd-dddd 或 ddd dd dddd）格式化的 SSN

  - Func_randomized_unformatted_ssn 查找 2011 年后未格式化为 9 个连续数字 (ddddddddd) 的 SSN

- **[校验和：](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** 否，没有校验和

- **[定义：](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** 如果在 300 个字符的邻近度内，DLP 策略 85% 确信它检测到这种类型的敏感信息：

  - [函数Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80)查找与模式匹配的内容。

  - 找到 [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) 中的一个关键字。 关键字的示例包括 *：Social Security、Social Security#、Soc Sec 、SSN。* 例如，以下示例将触发 DLP SSN 策略 **：SSN：489-36-8350**
  
有关内容需要检测 SSN 的内容详细信息，请参阅本文中的以下部分：敏感信息类型查找 [SSN 的内容](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
使用不同的内置敏感信息类型，请参阅以下文章，了解其他类型的信息：敏感信息 [类型查找什么](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  