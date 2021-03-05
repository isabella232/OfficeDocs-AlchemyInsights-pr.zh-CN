---
title: 了解谁在邮箱上设置了转发，以及如何
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464374"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a><span data-ttu-id="ab6b2-102">了解谁在邮箱上设置了转发，以及如何</span><span class="sxs-lookup"><span data-stu-id="ab6b2-102">Find out who set up forwarding on a mailbox, and how</span></span>

<span data-ttu-id="ab6b2-103">如果在邮箱上设置了外部转发，则活动作为 Set-Mailbox cmdlet 的一部分进行审核。</span><span class="sxs-lookup"><span data-stu-id="ab6b2-103">If external forwarding was set on a mailbox, the activity is audited as part of the Set-Mailbox cmdlet.</span></span> <span data-ttu-id="ab6b2-104">下面将了解如何在活动审核日志：</span><span class="sxs-lookup"><span data-stu-id="ab6b2-104">Here's how to find the activity in the audit log:</span></span>

1. <span data-ttu-id="ab6b2-105">转到 [Office 365 安全&合规中心](https://go.microsoft.com/fwlink/p/?linkid=2077143)。</span><span class="sxs-lookup"><span data-stu-id="ab6b2-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="ab6b2-106">选择 **"搜索** >  **审核日志搜索"。**</span><span class="sxs-lookup"><span data-stu-id="ab6b2-106">Select **Search**> **Audit log search**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="ab6b2-107">如果看到需要启用审核的通知，请继续，然后现在将其打开。</span><span class="sxs-lookup"><span data-stu-id="ab6b2-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="ab6b2-108">如果未启用此功能，搜索结果将无法从以前的日期提取数据。</span><span class="sxs-lookup"><span data-stu-id="ab6b2-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="ab6b2-109">请确保将 **"活动** "字段设置为" **显示** 默认活动 (活动) 。</span><span class="sxs-lookup"><span data-stu-id="ab6b2-109">Make sure the **Activities** field is set to **Show results for all activities** (the default).</span></span> <span data-ttu-id="ab6b2-110">指定日期范围。</span><span class="sxs-lookup"><span data-stu-id="ab6b2-110">Specify the date range.</span></span> <span data-ttu-id="ab6b2-111">无需指定用户名。</span><span class="sxs-lookup"><span data-stu-id="ab6b2-111">You don't need to specify a username.</span></span>
1. <span data-ttu-id="ab6b2-112">选择 **"搜索"。**</span><span class="sxs-lookup"><span data-stu-id="ab6b2-112">Select **Search**.</span></span> <span data-ttu-id="ab6b2-113">活动显示在"结果 **"下**。</span><span class="sxs-lookup"><span data-stu-id="ab6b2-113">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="ab6b2-114">选择 **"筛选** 结果"，然后在"活动筛选器"字段中 **输入\*\*\*\*Set-mailbox。**</span><span class="sxs-lookup"><span data-stu-id="ab6b2-114">Select **Filter Results**, and then enter **Set-mailbox** in the **Activity** filter field.</span></span> <span data-ttu-id="ab6b2-115">这将返回 **所有 Set-Mailbox** 活动。</span><span class="sxs-lookup"><span data-stu-id="ab6b2-115">This returns all **Set-Mailbox** activities.</span></span>
1. <span data-ttu-id="ab6b2-116">若要查看详细信息，请选择一个活动，然后选择 **"详细信息"。**</span><span class="sxs-lookup"><span data-stu-id="ab6b2-116">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="ab6b2-117">在 **"** 参数"下，可以看到邮箱上设置的转发电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="ab6b2-117">Under **Parameters** you can see the forwarding email address that was set on the mailbox.</span></span> <span data-ttu-id="ab6b2-118">**UserID** 表示在邮箱上设置外部转发的用户。</span><span class="sxs-lookup"><span data-stu-id="ab6b2-118">The **UserID** represents the user who set up external forwarding on the mailbox.</span></span>
<span data-ttu-id="ab6b2-119">若要了解更多信息，请参阅["搜索 Office 365 审核日志排查常见方案。](https://go.microsoft.com/fwlink/?linkid=2103944)</span><span class="sxs-lookup"><span data-stu-id="ab6b2-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>