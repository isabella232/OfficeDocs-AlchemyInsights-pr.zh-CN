---
title: DLP 未按预期正常工作
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
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0ed893420b5813d5d18639c2c226c12f0306a13f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679683"
---
# <a name="dlp-not-working-as-expected"></a>DLP 未按预期正常工作

**重要信息：** 在这段前所未有的时期，我们正在采取措施确保 SharePoint Online 和 OneDrive 服务高度可用，请访问 [SharePoint Online 临时功能调整](https://aka.ms/ODSPAdjustments)，获取详细信息。

 **设置 DLP**

您是否遇到 **数据丢失防护 (DLP) ** 在 Office 365 中的问题无法按预期工作？ 如果是这样，请确保您的 **dlp 策略** 设置正确，并且您的数据中包含 **DLP 策略** 在评估时要查找的内容。
  
DLP 策略允许你标识和保护组织中的敏感信息。 若要设置 DLP 策略，请使用 [此处](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)的信息。
  
 **DLP 策略查找的内容**
  
在安全与合规中心中使用 **内置的敏感信息类型** 时，DLP 策略会在检测到这些敏感类型时查找特定模式和元素。
  
- **内置的敏感信息类型**

    有关内置敏感类型以及在检测敏感类型时 DLP 策略查找的内容的信息，请参阅： [敏感信息类型查找的内容](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)。

- **自定义敏感信息类型**

    如果您尝试创建自定义敏感信息类型，请使用以下文章，了解有关如何创建自定义敏感信息类型的信息： [创建自定义敏感信息类型](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)。

**测试 DLP 策略**

若要使用内置或自定义的敏感信息类型测试数据，请使用 "**分类** **Test type**  >  **敏感信息类型**" 下的 "测试类型" 选项。 有关详细信息，请参阅 [测试自定义敏感信息类型](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)。

 **报表**
  
- 使用[DLP 报告](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)获取敏感数据见解。

- 有关事件 [报告](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)的详细信息，请参阅事件的具体详细信息。
