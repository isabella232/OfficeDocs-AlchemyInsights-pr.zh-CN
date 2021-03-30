---
title: 检查邮箱上的转发地址
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 3abd45230360c61ecb62e4b7a39d1b0b547271fc
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403301"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="bf593-102">检查邮箱上的转发地址</span><span class="sxs-lookup"><span data-stu-id="bf593-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="bf593-103">有时黑客将用户的电子邮件转发给自己，因此首先我们将检查邮箱上的转发地址和规则。</span><span class="sxs-lookup"><span data-stu-id="bf593-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="bf593-104">然后，我们将检查审核日志。</span><span class="sxs-lookup"><span data-stu-id="bf593-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="bf593-105">下面将了解如何检查转发地址：</span><span class="sxs-lookup"><span data-stu-id="bf593-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="bf593-106">选择 **"用户**  >  **""活动用户"。**</span><span class="sxs-lookup"><span data-stu-id="bf593-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="bf593-107">选择帐户遭到入侵的用户。</span><span class="sxs-lookup"><span data-stu-id="bf593-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="bf593-108">在出现的飞出控件中，展开"**邮件设置"，** 然后单击 **"编辑电子邮件\*\*\*\*转发"。**</span><span class="sxs-lookup"><span data-stu-id="bf593-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="bf593-109">删除你无法识别的任何转发地址。</span><span class="sxs-lookup"><span data-stu-id="bf593-109">Remove any forwarding addresses you don't recognize.</span></span>