---
title: DLP 可能需要自定义类型
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: c0996e0cc923c13b7de3752ac6534026e8627c51
ms.sourcegitcommit: dcd1c76ced1a0cec27f4cf8d383593760c198424
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2021
ms.locfileid: "59446681"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP 可能需要自定义类型

**重要信息：** 在这段前所未有的时期，我们正在采取措施确保 SharePoint Online 和 OneDrive 服务高度可用，请访问 [SharePoint Online 临时功能调整](https://aka.ms/ODSPAdjustments)，获取详细信息。

**DLP 可能需要自定义信息类型**

借助 DLP (策略) 数据丢失防护，您可以识别和保护您组织的敏感数据。 在某些情况下，可能需要创建自己的自定义敏感信息类型来保护组织的数据。 有关详细信息，请参阅[了解敏感信息类型和](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-learn-about)[敏感信息类型实体定义](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)。

若要详细了解如何创建自定义敏感信息类型和策略，请参阅： 

**自定义内置敏感信息类型**

如果只需做一些调整，内置敏感信息类型就能够满足你的需求，请参阅自定义 [内置敏感信息类型](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type)。 例如，可以添加或删除关键字，也可以添加或删除支持性证据，如日期或地址。

**创建自定义敏感信息类型**

但是，如果需要完全标识和保护不同类型的敏感信息，可以在该模板中创建自定义Microsoft 365 合规中心。 有关详细信息，请参阅自定义 [敏感信息类型入门](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type)。

**使用安全与合规中心 PowerShell 创建自定义敏感信息类型**

最后，如果用户界面未提供您所需的全部选项，您可以在安全与合规中心 PowerShell &敏感信息类型。 从 XML 文件开始，可以使用每个可用的选项。 有关详细信息，请参阅使用 [PowerShell 创建自定义敏感信息类型](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell)。

若要首先在测试模式下测试策略，请参阅 [在](https://docs.microsoft.com/microsoft-365/compliance/dlp-learn-about-dlp#implement-policy-in-test-mode) 测试模式下实现策略和 [创建、测试和调整 DLP 策略](https://docs.microsoft.com/microsoft-365/compliance/create-test-tune-dlp-policy)。 