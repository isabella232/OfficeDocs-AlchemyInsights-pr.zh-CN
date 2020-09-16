---
title: 2419-无法启用-审核
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 81fd8e33feb2f2b10b04cc7cdc746a8603aa366b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767589"
---
# <a name="unable-to-enable-unified-auditing"></a><span data-ttu-id="a0786-102">无法启用统一审核</span><span class="sxs-lookup"><span data-stu-id="a0786-102">Unable to enable unified auditing</span></span>

<span data-ttu-id="a0786-103">当您尝试为您的组织启用统一审核时，您可能会收到类似于以下的错误：</span><span class="sxs-lookup"><span data-stu-id="a0786-103">When you try to enable unified auditing for your organization, you may receive an error similar the following:</span></span>

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

<span data-ttu-id="a0786-104">若要解决此问题，请按照下列步骤操作：</span><span class="sxs-lookup"><span data-stu-id="a0786-104">To resolve this issue, follow these steps:</span></span>

1. <span data-ttu-id="a0786-105">[连接到 Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)。</span><span class="sxs-lookup"><span data-stu-id="a0786-105">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="a0786-106">运行以下 cmdlet：</span><span class="sxs-lookup"><span data-stu-id="a0786-106">Run the following cmdlet:</span></span>

   ```
   Enable-OrganizationCustomization
   ```

3. <span data-ttu-id="a0786-107">等待60分钟后，上一设置才会生效。</span><span class="sxs-lookup"><span data-stu-id="a0786-107">Wait for 60 minutes for the previous setting to take effect.</span></span>

4. <span data-ttu-id="a0786-108">在 Exchange Online PowerShell 中运行以下命令：</span><span class="sxs-lookup"><span data-stu-id="a0786-108">Run the following command in Exchange Online PowerShell:</span></span>

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

<span data-ttu-id="a0786-109">有关其他信息，请参阅以下文章：</span><span class="sxs-lookup"><span data-stu-id="a0786-109">For additional information, see the following articles:</span></span>

- [<span data-ttu-id="a0786-110">使用多重身份验证连接到 Exchange Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="a0786-110">Connect to Exchange Online PowerShell using multi-factor authentication</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [<span data-ttu-id="a0786-111">启用或禁用审核日志搜索</span><span class="sxs-lookup"><span data-stu-id="a0786-111">Turn audit log search on or off</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
