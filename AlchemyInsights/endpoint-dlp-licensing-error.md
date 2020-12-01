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
ms.openlocfilehash: d17c51177898d62c7c477460c8c26b4753bae65f
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2020
ms.locfileid: "49477646"
---
# <a name="endpoint-dlp-licensing-error"></a>终结点 DLP 许可错误

尝试设置终结点 DLP 时，如果收到以下错误：

`Your organization is missing the licenses required to manage these devices`.

确保您具有以下订阅或加载项之一：

- Microsoft 365 E5
- Microsoft 365 A5 (EDU)
- Microsoft 365 E5 合规
- Microsoft 365 A5 合规
- Microsoft 365 E5 信息保护和治理
- Microsoft 365 A5 信息保护和治理

> [!NOTE]
> 这将不适用于许可证组合，如 Win E5 + O365 E5 + EMS E5。 若要设置此功能，您必须具有一个纯 M365 E5 许可证。

有关 Endpoint DLP 许可的详细信息，请参阅 [ENDPOINT DLP 许可。](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)
