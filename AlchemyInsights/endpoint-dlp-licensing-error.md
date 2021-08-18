---
title: 终结点 DLP 许可错误
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200001"
- "7176"
ms.openlocfilehash: c32ab88a72c265be411350e50756f5b2e1e3337c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58322121"
---
# <a name="endpoint-dlp-licensing-error"></a>终结点 DLP 许可错误

尝试设置 Endpoint DLP 时，如果您收到以下错误：

`Your organization is missing the licenses required to manage these devices`.

确保你具有以下订阅或加载项之一：

- Microsoft 365 E5
- Microsoft 365 A5 (EDU)
- Microsoft 365 E5 合规
- Microsoft 365 A5 合规
- Microsoft 365 E5 信息保护和治理
- Microsoft 365 A5 信息保护和治理

**注意**：这适用于许可证组合，例如：Win E5 + O365 E5 + EMS E5。 您必须拥有纯 M365 E5 许可证才能设置此功能。

有关终结点 DLP 许可信息，请参阅 [Endpoint DLP Licensing。](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)
