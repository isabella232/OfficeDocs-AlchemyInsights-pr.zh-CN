---
title: 932 升级 AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 9582f1f56e6730e35520b5d79bc245cd74bea0bf4db39b379a7cd133bafc16ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104802"
---
# <a name="upgrade-azure-ad-connect"></a>升级 Azure AD 连接

默认情况下，为 Azure AD 连接启用自动升级，这有助于确保你运行的是最新版本。 若要验证自动升级设置，请使用 Azure AD PowerShell 中的 **Get-ADSyncAutoUpgrade** cmdlet。 此 cmdlet 将返回下列值之一：

- **已启用**：启用自动升级。

- **已禁用**：自动升级处于禁用状态。

- **Suspended**：系统不再有资格接收自动升级。 无法配置此值;它由系统设置。

有关详细信息，请参阅自动 [升级](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)。

若要下载最新版 Azure AD 连接，请转到 [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) 。
