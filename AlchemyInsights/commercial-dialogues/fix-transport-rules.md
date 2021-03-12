---
title: 修复传输规则
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736152"
---
# <a name="fix-transport-rules"></a><span data-ttu-id="bcb2d-102">修复传输规则</span><span class="sxs-lookup"><span data-stu-id="bcb2d-102">Fix transport rules</span></span>

<span data-ttu-id="bcb2d-103">自定义邮件流规则影响此邮件。</span><span class="sxs-lookup"><span data-stu-id="bcb2d-103">A custom mail flow rule affected this message.</span></span> <span data-ttu-id="bcb2d-104">若要查看确切的规则，请执行下列操作：</span><span class="sxs-lookup"><span data-stu-id="bcb2d-104">To review the exact rule, do the following:</span></span>

1. <span data-ttu-id="bcb2d-105">在提交结果中的" **其他信息"下**，记下 **GUID** 或 **策略名称**。</span><span class="sxs-lookup"><span data-stu-id="bcb2d-105">In the submission results, under **Additional information**, note the **GUID** or the **Policy Name**.</span></span>
2. <span data-ttu-id="bcb2d-106">启动 Exchange 命令行管理程序。</span><span class="sxs-lookup"><span data-stu-id="bcb2d-106">Launch Exchange Management Shell.</span></span> <span data-ttu-id="bcb2d-107">有关详细信息，请参阅[Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432)。</span><span class="sxs-lookup"><span data-stu-id="bcb2d-107">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
3. <span data-ttu-id="bcb2d-108">使用提交 (GUID 运行此命令  **) ：Get-TransportRule -identity "GUID" | fl \* Description**\*</span><span class="sxs-lookup"><span data-stu-id="bcb2d-108">Run this command (using the GUID from your submission):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span></span>
4. <span data-ttu-id="bcb2d-109">查看说明以查看影响邮件的已配置条件。</span><span class="sxs-lookup"><span data-stu-id="bcb2d-109">Review the description to see the configured conditions that affected the message.</span></span>

<span data-ttu-id="bcb2d-110">若要了解更多信息，请参阅 [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523)。</span><span class="sxs-lookup"><span data-stu-id="bcb2d-110">To learn more, see [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span></span>
