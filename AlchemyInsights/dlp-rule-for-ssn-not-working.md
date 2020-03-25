---
title: SSN 的 DLP 规则不起作用
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 0b83a858975ffe1bb70f16a7452a13d57dff5340
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932511"
---
# <a name="dlp-issues-with-social-security-numbers"></a>包含社会保险号的 DLP 问题

**重要说明**：许多 SharePoint Online 和 OneDrive 客户对在后台运行的服务运行关键业务应用程序。 其中包括内容迁移、数据丢失防护（DLP）和备份解决方案。 在这些前所未有的时间内，我们将采取措施，以确保在远程工作方案中，SharePoint Online 和 OneDrive 服务对依赖于该服务的用户保持高可用性和可靠性。

为支持此目标，我们已在工作日白天营业时对后台应用（迁移、DLP 和备份解决方案）实施了更严格的限制限制。 在这些情况中，您应认为这些应用程序的吞吐量非常有限。 但是，在夜间和周末的时间内，服务将准备好处理来自后台应用程序的较大数量的请求。

**Ssn 的 DLP 问题**

在使用 Office 365 中的敏感信息类型时，您是否遇到**数据丢失防护（DLP）** 无法处理包含**社会保险号码（SSN）** 的内容的问题？ 如果是这样，请确保您的内容包含 DLP 策略所需的信息所需的信息。 
  
例如，对于配置为可信度为85% 的 SSN 策略，将对以下项进行评估，并且必须检测到规则才能触发：
  
- **[格式：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 个数字，可以是格式化或无格式的模式

- **[模式：](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** 四个函数在四种不同的模式中查找 Ssn：

  - Func_ssn 查找具有 2011 年以前使用短划线或空格格式化的强格式的 SSN（ddd-dd-dddd 或 ddd dd dddd）

  - Func_unformatted_ssn 查找具有 2011 年以前未格式化为 9 个连续数字的强格式的 SSN (ddddddddd)

  - Func_randomized_formatted_ssn 查找 2011 年后使用短划线或空格（ddd-dd-dddd 或 ddd dd dddd）格式化的 SSN

  - Func_randomized_unformatted_ssn 查找 2011 年后未格式化为 9 个连续数字 (ddddddddd) 的 SSN

- **[校验和：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** 否，没有校验和

- **[定义：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** 如果 DLP 策略在300个字符的邻近度内检测到此类型的敏感信息，则 DLP 策略85% 确信它检测到这种类型的敏感信息：

  - [函数 Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)找到与该模式匹配的内容。

  - 找到 [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) 中的一个关键字。 关键字的示例包括：*社会保险、社会 security #、Soc Sec、SSN* 。 例如，以下示例将触发 DLP SSN 策略： **SSN： 489-36-8350**
  
若要详细了解为您的内容检测 Ssn 所需的信息，请参阅本文中的以下部分：[敏感信息类型查找的内容 ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
使用不同的内置敏感信息类型，请参阅以下文章，了解其他类型所需的信息：[敏感信息类型查找的内容](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  