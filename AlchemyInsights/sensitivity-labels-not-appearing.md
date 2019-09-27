---
title: 敏感度标签未显示
ms.author: stephow
author: stephow-MSFT
manager: laurawi
ms.date: ''
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 4bf8e02246c966f22648467386a7862f0521fecf
ms.sourcegitcommit: 71978e2bb779b5955fd113f84512b83321b26912
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37207215"
---
# <a name="sensitivity-labels-not-appearing"></a>敏感度标签未显示

敏感度标签允许您对敏感内容进行分类和帮助保护。 可以在 Microsoft 365 合规性中心、Microsoft 365 安全中心或 Office 365 安全 & 合规性中心下的 "分类 > 敏感度标签" 下创建它们。 若要了解有关此功能的详细信息，请参阅[敏感度标签概述](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels)。

如果您配置了灵敏度标签但它们未显示在 Office 应用中，请检查以下各项：

- 确认是否已将敏感度标签[发布](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do)到所需的用户和组。

- 确认用户正在使用支持敏感度标签的应用程序-请参阅[文档中的敏感度标签](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?ad=US&ui=en-US&rs=en-US#bkmk_whereavailable)。

- 如果要[迁移 Azure 信息保护标签](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)，请注意[此处](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)列出的注意事项。

- 数据丢失防护（DLP）支持：目前，在 DLP 策略中，仅保留标签可用作条件。  DLP 策略中的敏感度标签支持尚不可用，但我们正在对其进行处理。

- 对敏感度标签启用加密时，您可以选择执行以下操作之一：
    - 立即分配权限
    - 允许用户分配权限


有关可能存在的问题的详细信息，请参阅[灵敏度标签的已知问题](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc)。