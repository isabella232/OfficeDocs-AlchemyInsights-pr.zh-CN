---
title: '修复租户策略 (替代) '
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
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2021
ms.locfileid: "50552280"
---
# <a name="fix-tenant-policy-action-override"></a><span data-ttu-id="5dbbe-102">修复租户策略 (替代) </span><span class="sxs-lookup"><span data-stu-id="5dbbe-102">Fix Tenant policy (action override)</span></span>

<span data-ttu-id="5dbbe-103">租户中的反垃圾邮件策略影响此邮件。</span><span class="sxs-lookup"><span data-stu-id="5dbbe-103">An anti-spam policy in your tenant affected this message.</span></span> <span data-ttu-id="5dbbe-104">若要查看策略，请执行下列操作：</span><span class="sxs-lookup"><span data-stu-id="5dbbe-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="5dbbe-105">转到 [Office 365 安全&](https://go.microsoft.com/fwlink/p/?linkid=2077143)合规中心，然后转到 **"威胁管理**  >  **策略**  >  [反垃圾邮件"。](https://go.microsoft.com/fwlink/?linkid=2101518)</span><span class="sxs-lookup"><span data-stu-id="5dbbe-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="5dbbe-106">检查策略源 **是否** 指示以下内容  **：Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC 邮件**</span><span class="sxs-lookup"><span data-stu-id="5dbbe-106">Check to see if **Policy source** indicates the following:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**</span></span>

    <span data-ttu-id="5dbbe-107">如果是，请在" **自定义** "选项卡上检查影响邮件的策略的设置。</span><span class="sxs-lookup"><span data-stu-id="5dbbe-107">If so, on the **Custom** tab, check the settings of the policy that affected the message.</span></span> <span data-ttu-id="5dbbe-108">应用于所有 Exchange Online Protection 客户的 **标准** 设置可能会影响邮件。</span><span class="sxs-lookup"><span data-stu-id="5dbbe-108">It's possible that the **Standard settings** applied to all Exchange Online Protection customers affected the message.</span></span>

<span data-ttu-id="5dbbe-109">有关配置垃圾邮件筛选器策略的信息，请参阅["配置垃圾邮件筛选器策略"。](https://go.microsoft.com/fwlink/?linkid=2101431)</span><span class="sxs-lookup"><span data-stu-id="5dbbe-109">For more information on configuring spam filter policies, see [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).</span></span>
