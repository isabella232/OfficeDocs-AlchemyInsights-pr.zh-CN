---
title: DLP 未如预期工作
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
ms.openlocfilehash: 0f07e64c95675a4f6a0aeb6df110fe4e6a21d72f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707800"
---
# <a name="dlp-not-working-as-expected"></a>DLP 未如预期工作

**重要信息：** 在这段前所未有的时期，我们正在采取措施确保 SharePoint Online 和 OneDrive 服务高度可用，请访问 [SharePoint Online 临时功能调整](https://aka.ms/ODSPAdjustments)，获取详细信息。

 **设置 DLP**

Office 365 中的 **数据丢失防护 (DLP)** 是否未如预期工作？ 如果是，请确保 **DLP** 策略设置正确，并且数据包含 **DLP** 策略在评估时正在查找的内容。
  
DLP 策略允许您标识和保护您组织的敏感信息。 若要设置 DLP 策略，请使用此处 [的信息](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template)。
  
 **DLP 策略查找什么**
  
在安全与合规中心内使用内置敏感信息类型时，DLP 策略在检测这些敏感信息类型时会查找特定模式和元素。
  
- **内置敏感信息类型**

    有关内置敏感类型以及 DLP 策略在检测敏感类型时查找的信息，请参阅：敏感信息类型 [查找什么](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)。

- **自定义敏感信息类型**

    如果您尝试创建自定义敏感信息类型，请使用以下文章来了解如何创建自定义敏感信息类型： [创建自定义敏感信息类型](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)。

**测试 DLP 策略**

若要使用内置或自定义敏感信息类型测试数据，请使用分类敏感信息类型下的"测试  >  **类型"选项**。 有关详细信息，请参阅["测试自定义敏感信息类型"。](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)

 **报表**
  
- 使用 DLP 报告获取 [敏感数据见解。](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- 使用事件报告查看事件 [的特定详细信息](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)。
