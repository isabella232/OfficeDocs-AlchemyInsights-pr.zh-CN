---
title: 2419-无法启用-审核
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 3af01c03711eed646f0009afb5bea685bc358196
ms.sourcegitcommit: 87153fec6f6468b57893abf4aac073ba4068e67b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2019
ms.locfileid: "35065605"
---
# <a name="unable-to-enable-unified-auditing"></a><span data-ttu-id="4cb86-102">无法启用统一审核</span><span class="sxs-lookup"><span data-stu-id="4cb86-102">Unable to enable unified auditing</span></span>

<span data-ttu-id="4cb86-103">当您尝试为您的 Office 365 组织启用统一审核时, 您可能会收到类似于以下的错误:</span><span class="sxs-lookup"><span data-stu-id="4cb86-103">When you try to enable unified auditing for your Office 365 organization, you may receive an error similar the following:</span></span>

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

<span data-ttu-id="4cb86-104">若要解决此问题, 请按照下列步骤操作:</span><span class="sxs-lookup"><span data-stu-id="4cb86-104">To resolve this issue, follow these steps:</span></span>

1. <span data-ttu-id="4cb86-105">[连接到 Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)。</span><span class="sxs-lookup"><span data-stu-id="4cb86-105">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="4cb86-106">运行以下 cmdlet：</span><span class="sxs-lookup"><span data-stu-id="4cb86-106">Run the following cmdlet:</span></span>

   ```
   Enable-OrganizationCustomization
   ```

3. <span data-ttu-id="4cb86-107">等待60分钟后, 上一设置才会生效。</span><span class="sxs-lookup"><span data-stu-id="4cb86-107">Wait for 60 minutes for the previous setting to take effect.</span></span>

4. <span data-ttu-id="4cb86-108">在 Exchange Online PowerShell 中运行以下命令:</span><span class="sxs-lookup"><span data-stu-id="4cb86-108">Run the following command in Exchange Online PowerShell:</span></span>

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

<span data-ttu-id="4cb86-109">有关其他信息, 请参阅以下文章:</span><span class="sxs-lookup"><span data-stu-id="4cb86-109">For additional information, see the following articles:</span></span>

- [<span data-ttu-id="4cb86-110">使用多重身份验证连接到 Exchange Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="4cb86-110">Connect to Exchange Online PowerShell using multi-factor authentication</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [<span data-ttu-id="4cb86-111">启用或禁用 Office 365 审核日志搜索</span><span class="sxs-lookup"><span data-stu-id="4cb86-111">Turn Office 365 audit log search on or off</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)
