---
title: 测试新 OME 功能的 IRM 配置
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12428"
- "9000078"
ms.openlocfilehash: d084caabfbcfdd92d6b90554c9e2bef5f571a0227827332a5fb3d710d7bc4836
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/11/2021
ms.locfileid: "57899686"
---
# <a name="test-irm-configuration-for-new-ome-capabilities"></a>测试新 OME 功能的 IRM 配置

若要验证 Microsoft 365 租户是否配置为使用新的 OME 功能，请在连接到 [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online-powershell) 时运行以下 cmdlet:


1. 通过运行 `Get-IRMConfiguration` 来检查租户的 IRM 配置。 请确保这些值设置为 **True**:
    
    **InternalLicensingEnabled**
    
    **ExternalLicensingEnabled**
    
    **AzureRMSLicensingEnabled**

2. 使用域、发件人地址和收件人运行 `Test-IRMConfiguration`。 如果测试未通过，请调查 IRM 配置。

有关如何验证 IRM 配置的详细信息，请参阅 [在 Exchange Online PowerShell 中验证新的 OME 配置](https://docs.microsoft.com/microsoft-365/compliance/set-up-new-message-encryption-capabilities#verify-new-ome-configuration-in-exchange-online-powershell)。