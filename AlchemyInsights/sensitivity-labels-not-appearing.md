---
title: 未显示敏感度标签
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 824824257fee4aaaab1f2dd32597b4cdc858d035fabd357af90cf054dd35c9c4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061422"
---
# <a name="sensitivity-labels-not-appearing"></a>未显示敏感度标签

敏感度标签允许你对敏感内容进行分类和保护。 可以在安全中心、安全Microsoft 365 合规中心Microsoft 365安全中心Microsoft 365分类&敏感度标签>创建它们。 若要了解有关此功能的信息，请参阅 [敏感度标签概述](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)。

如果你已配置敏感度标签，但它们未显示在Microsoft 365应用中，请检查以下各项：

- 确认敏感度标签已发布 [到](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) 您需要的用户和组。

- 确认用户使用的是支持敏感度标签的应用 ，请参阅 [文档中的敏感度标签](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable)。

- 如果要迁移 [Azure 信息保护标签](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)，请注意此处列出的 [注意事项](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)。

- DLP 支持 (数据丢失) ：目前，只有保留标签可以用作 DLP 策略中的条件。  尚不支持 DLP 策略中的敏感度标签，但我们正在努力进行。

- 在敏感度标签上启用加密后，可以选择：
    - 立即分配权限
    - 允许用户分配权限


有关可能的问题详细信息，请参阅敏感度 [标签的已知问题](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc)。