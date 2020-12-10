---
title: '语音邮件疑难解答 '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7564"
ms.openlocfilehash: a2d26da512838ae112c352fe21366074b69fa224
ms.sourcegitcommit: 3802f2f4db4f53a408a360187db67f2296448c21
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607993"
---
# <a name="troubleshooting-voicemail"></a><span data-ttu-id="983c9-102">语音邮件疑难解答</span><span class="sxs-lookup"><span data-stu-id="983c9-102">Troubleshooting Voicemail</span></span>

<span data-ttu-id="983c9-103">确保 "忙碌忙" 功能是特意的。</span><span class="sxs-lookup"><span data-stu-id="983c9-103">Ensure that the Busy on Busy feature is intentional.</span></span>

<span data-ttu-id="983c9-104">如果此用户不需要此功能，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="983c9-104">If this feature is not needed on this user:</span></span>

1. <span data-ttu-id="983c9-105">转到 " [团队" 管理中心](https://admin.teams.microsoft.com/policies/calling)。</span><span class="sxs-lookup"><span data-stu-id="983c9-105">Go to [Teams Admin center](https://admin.teams.microsoft.com/policies/calling).</span></span>
1. <span data-ttu-id="983c9-106">在左滑轨上，浏览 **语音**  >  **呼叫策略**  >  **管理\*\*\*\*呼叫策略** 上的策略。</span><span class="sxs-lookup"><span data-stu-id="983c9-106">On the left rail navigate **Voice** > **Calling policies** > **Manage Policies** on the **Calling Policy**.</span></span>
1. <span data-ttu-id="983c9-107">选择 " **管理用户**"。</span><span class="sxs-lookup"><span data-stu-id="983c9-107">Select **Manage Users**.</span></span>
1. <span data-ttu-id="983c9-108">**在呼叫 "关闭" 时**，搜索用户并将呼叫策略更改为忙闲的呼叫策略可用。 </span><span class="sxs-lookup"><span data-stu-id="983c9-108">Search for user and change the Calling Policy to one that has **Busy on Busy is available when in a call** to **Off**.</span></span>
1. <span data-ttu-id="983c9-109">单击“**应用**”。</span><span class="sxs-lookup"><span data-stu-id="983c9-109">Click **Apply**.</span></span>
> [!NOTE]
> <span data-ttu-id="983c9-110">对策略所做的更改可能需要长达24小时才能进行复制。</span><span class="sxs-lookup"><span data-stu-id="983c9-110">Changes to policies can take up to 24 hours to replicate.</span></span>

<span data-ttu-id="983c9-111">有关此功能的详细信息，请参阅： [在呼叫中时忙闲状态可用](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call)。</span><span class="sxs-lookup"><span data-stu-id="983c9-111">For more information on this feature refer to: [Busy on Busy is available while in a call](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span></span>
