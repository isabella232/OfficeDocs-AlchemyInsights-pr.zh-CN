---
title: 查找对收件箱规则执行的事件
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
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464503"
---
# <a name="find-events-performed-on-inbox-rules"></a><span data-ttu-id="9ea72-102">查找在收件箱规则上执行的事件</span><span class="sxs-lookup"><span data-stu-id="9ea72-102">Find events performed on inbox rules</span></span>

<span data-ttu-id="9ea72-103">创建、更改或删除收件箱规则时，事件将记录在审核日志。</span><span class="sxs-lookup"><span data-stu-id="9ea72-103">When inbox rules are created, changed, or deleted, the events are recorded in the audit log.</span></span> <span data-ttu-id="9ea72-104">下面将了解如何查看它们：</span><span class="sxs-lookup"><span data-stu-id="9ea72-104">Here's how to review them:</span></span>

1. <span data-ttu-id="9ea72-105">转到 [Office 365 安全&合规中心](https://go.microsoft.com/fwlink/p/?linkid=2077143)。</span><span class="sxs-lookup"><span data-stu-id="9ea72-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="9ea72-106">选择">审核日志搜索"。</span><span class="sxs-lookup"><span data-stu-id="9ea72-106">Select Search > Audit log search.</span></span>

    > [!NOTE]
    > <span data-ttu-id="9ea72-107">如果看到需要启用审核的通知，请继续，然后现在将其打开。</span><span class="sxs-lookup"><span data-stu-id="9ea72-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="9ea72-108">如果未启用此功能，搜索结果将无法从以前的日期提取数据。</span><span class="sxs-lookup"><span data-stu-id="9ea72-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="9ea72-109">选择"活动"字段并查找 Exchange 邮箱活动，然后选择New-InboxRule创建收件箱规则Outlook Web App。</span><span class="sxs-lookup"><span data-stu-id="9ea72-109">Select the Activities field and find Exchange mailbox activities, and then select New-InboxRule Create inbox rule from Outlook Web App.</span></span> <span data-ttu-id="9ea72-110">完成后，单击窗格外部以最小化"活动"窗格。</span><span class="sxs-lookup"><span data-stu-id="9ea72-110">When you're done, click outside of the pane to minimize the Activities pane.</span></span>
1. <span data-ttu-id="9ea72-111">指定日期范围，然后在"用户"字段中，选择要调查的用户的用户名。</span><span class="sxs-lookup"><span data-stu-id="9ea72-111">Specify the date range, and then in the Users field, select the username for the user you want to investigate.</span></span> <span data-ttu-id="9ea72-112">一次可以选择多个用户。</span><span class="sxs-lookup"><span data-stu-id="9ea72-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="9ea72-113">选择"搜索"。</span><span class="sxs-lookup"><span data-stu-id="9ea72-113">Select Search.</span></span> <span data-ttu-id="9ea72-114">活动显示在"结果"下。</span><span class="sxs-lookup"><span data-stu-id="9ea72-114">The activities appear under Results.</span></span>
1. <span data-ttu-id="9ea72-115">若要查看详细信息，请选择活动，然后选择"详细信息"。</span><span class="sxs-lookup"><span data-stu-id="9ea72-115">To view details, select an activity, and then select More Information.</span></span> <span data-ttu-id="9ea72-116">在"参数"部分，你可以看到规则的名称、条件集以及规则将采取的操作。</span><span class="sxs-lookup"><span data-stu-id="9ea72-116">Under the Parameters section you can see the name of the rule, conditions set, and the actions that the rule will take.</span></span>

<span data-ttu-id="9ea72-117">若要了解更多信息，请参阅"搜索 Office 365 审核日志排查常见方案问题。</span><span class="sxs-lookup"><span data-stu-id="9ea72-117">To learn more, see Search the Office 365 audit log to troubleshoot common scenarios.</span></span>