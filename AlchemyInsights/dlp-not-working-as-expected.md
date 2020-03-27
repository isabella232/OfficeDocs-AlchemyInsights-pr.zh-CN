---
title: DLP 未按预期正常工作
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 574a8a43d8264e98c6af2bfeb1bb472475e6e334
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977428"
---
# <a name="dlp-not-working-as-expected"></a>DLP 未按预期正常工作

**重要说明**：在这些前所未有的时间内，我们将采取措施来确保 sharepoint Online 和 OneDrive 服务保持高可用性-有关详细信息，请参阅[Sharepoint Online 临时功能调整](https://aka.ms/ODSPAdjustments)。

 **设置 DLP**

Office 365 中的**数据丢失防护（DLP）** 是否有问题无法按预期工作？ 如果是这样，请确保您的**dlp 策略**设置正确，并且您的数据中包含**DLP 策略**在评估时要查找的内容。
  
DLP 策略允许你标识和保护组织中的敏感信息。 若要设置 DLP 策略，请使用[此处](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)的信息。
  
 **DLP 策略查找的内容**
  
在 Office 365 安全与合规中心中使用**内置的敏感信息类型**时，DLP 策略会在检测这些敏感类型时查找特定模式和元素。
  
- **内置的敏感信息类型**

    有关内置敏感类型以及在检测敏感类型时 DLP 策略查找的内容的信息，请参阅：[敏感信息类型查找的内容](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)。

- **自定义敏感信息类型**

    如果您尝试创建自定义敏感信息类型，请使用以下文章，了解有关如何创建自定义敏感信息类型的信息：[创建自定义敏感信息类型](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)。

**测试 DLP 策略**

若要使用内置或自定义的敏感信息类型测试数据，请使用 "**分类** > **敏感信息类型**" 下的 "**测试类型**" 选项。 有关详细信息，请参阅[测试自定义敏感信息类型](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center)。

 **报表**
  
- 使用[DLP 报告](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)获取敏感数据见解。

- 有关事件[报告](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports)的详细信息，请参阅事件的具体详细信息。
