---
title: 检查邮箱上的转发地址
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 17/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 1b0a6c8fe368196f2d1f9811aea895c2c024b2e6
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416962"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="00fbd-102">检查邮箱上的转发地址</span><span class="sxs-lookup"><span data-stu-id="00fbd-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="00fbd-103">有时黑客将用户的电子邮件转发给自己，因此首先我们将检查邮箱上的转发地址和规则。</span><span class="sxs-lookup"><span data-stu-id="00fbd-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="00fbd-104">然后，我们将检查审核日志。</span><span class="sxs-lookup"><span data-stu-id="00fbd-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="00fbd-105">下面是如何检查转发地址的：</span><span class="sxs-lookup"><span data-stu-id="00fbd-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="00fbd-106">选择 **"**  >  **用户活动用户"。**</span><span class="sxs-lookup"><span data-stu-id="00fbd-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="00fbd-107">选择帐户已被泄露的用户。</span><span class="sxs-lookup"><span data-stu-id="00fbd-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="00fbd-108">在出现的飞出控件中，展开 **"邮件设置**"，然后单击 **"编辑电子邮件\*\*\*\*转发"。**</span><span class="sxs-lookup"><span data-stu-id="00fbd-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="00fbd-109">删除你无法识别的任何转发地址。</span><span class="sxs-lookup"><span data-stu-id="00fbd-109">Remove any forwarding addresses you don't recognize.</span></span>