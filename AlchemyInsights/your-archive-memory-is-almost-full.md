---
title: 存档邮箱几乎已满
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/25/2021
ms.locfileid: "49950503"
---
# <a name="your-archive-mailbox-is-almost-full"></a><span data-ttu-id="f6f11-102">存档邮箱几乎已满</span><span class="sxs-lookup"><span data-stu-id="f6f11-102">Your archive mailbox is almost full</span></span>

<span data-ttu-id="f6f11-103">如果用户收到警告; **您的存档邮箱几乎已满**，或者您需要增加存档邮箱的大小，以下是一些提示：</span><span class="sxs-lookup"><span data-stu-id="f6f11-103">If the user receives the warning; **Your archive mailbox is almost full**, or you need to increase the size of their archive mailbox, here are some tips:</span></span>

1. <span data-ttu-id="f6f11-104">如果为用户分配了 Exchange Online 计划 1，请升级到 **Exchange Online 计划 2** 许可证，以将大小从 50 GB 增加至 100GB。</span><span class="sxs-lookup"><span data-stu-id="f6f11-104">If the user is assigned an Exchange Online Plan 1, upgrade to **Exchange Online Plan 2** license to increase the size from 50 GB to 100GB.</span></span>
1. <span data-ttu-id="f6f11-105">如果用户已分配有以下任一项 **：Exchange Online 计划 2** 或具有 Exchange Online Archiving 加载项的 Exchange Online 计划 1，请使用以下步骤启用自动扩展存档：。</span><span class="sxs-lookup"><span data-stu-id="f6f11-105">If the user is already assigned either of the following: **Exchange Online Plan 2** or an Exchange Online Plan 1 with an Exchange Online Archiving add-on, use the steps below to enable Auto-Expanding archiving:.</span></span>
 
    1. <span data-ttu-id="f6f11-106">[连接到 Exchange Online Powershell。](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="f6f11-106">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span></span>
    2. <span data-ttu-id="f6f11-107">为用户运行以下命令let：  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span><span class="sxs-lookup"><span data-stu-id="f6f11-107">Run the following commandlet for the user:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span></span>
    1. <span data-ttu-id="f6f11-108">运行以下命令let 以确认用户已启用：  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span><span class="sxs-lookup"><span data-stu-id="f6f11-108">Run the following commandlet to confirm it is enabled for the user:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span></span>

<span data-ttu-id="f6f11-109">有关详细信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="f6f11-109">For more information see:</span></span>

- [<span data-ttu-id="f6f11-110"> 启用无限制存档 - 管理员帮助 - Microsoft 365 合规性|Microsoft Docs</span><span class="sxs-lookup"><span data-stu-id="f6f11-110"> Enable unlimited archiving - Admin Help - Microsoft 365 Compliance | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [<span data-ttu-id="f6f11-111">Exchange Online 限制 - 服务说明|Microsoft Docs</span><span class="sxs-lookup"><span data-stu-id="f6f11-111">Exchange Online limits - Service Descriptions | Microsoft Docs</span></span>](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [<span data-ttu-id="f6f11-112">升级到其他业务计划|Microsoft Docs</span><span class="sxs-lookup"><span data-stu-id="f6f11-112">Upgrade to a different business plan | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

