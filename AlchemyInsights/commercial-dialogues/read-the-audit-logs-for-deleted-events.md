---
title: 读取已删除事件的审核日志
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
ms.openlocfilehash: 9739fb1eb8e4f5adf81cd699c851a51176f0429e
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464370"
---
# <a name="read-the-audit-logs-for-deleted-events"></a><span data-ttu-id="d9579-102">读取已删除事件的审核日志</span><span class="sxs-lookup"><span data-stu-id="d9579-102">Read the audit logs for deleted events</span></span>

<span data-ttu-id="d9579-103">下面是如何进行此操作：</span><span class="sxs-lookup"><span data-stu-id="d9579-103">Here's how to do this:</span></span>

1. <span data-ttu-id="d9579-104">转到 [Office 365 安全&合规中心](https://go.microsoft.com/fwlink/p/?linkid=2077143)。</span><span class="sxs-lookup"><span data-stu-id="d9579-104">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="d9579-105">选择 **"搜索**  >  [**审核日志搜索"。**](https://go.microsoft.com/fwlink/?linkid=2103759)</span><span class="sxs-lookup"><span data-stu-id="d9579-105">Select **Search** > [**Audit log search**](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>
    > [!NOTE]
    > <span data-ttu-id="d9579-106">如果看到需要打开该功能的通知，请继续，然后现在将其打开。</span><span class="sxs-lookup"><span data-stu-id="d9579-106">If you see a notice that you need to turn on the feature, go ahead and turn it on now.</span></span> <span data-ttu-id="d9579-107">如果未启用此功能，搜索结果将无法从以前的日期提取数据。</span><span class="sxs-lookup"><span data-stu-id="d9579-107">If the feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="d9579-108">选择 **"** 活动"，然后查找 **Exchange 邮箱活动**。</span><span class="sxs-lookup"><span data-stu-id="d9579-108">Select **Activities**, and then find **Exchange mailbox activities**.</span></span> <span data-ttu-id="d9579-109">选择 **"已删除邮件"文件夹中的** "已删除邮件"和"将邮件 **移动到已删除邮件"** 文件夹选项。</span><span class="sxs-lookup"><span data-stu-id="d9579-109">Select the **Deleted messages from Deleted Items** folder and **Moved messages to Deleted Items** folder options.</span></span> <span data-ttu-id="d9579-110">完成后，单击窗格外部以最小化 **"活动"** 窗格。</span><span class="sxs-lookup"><span data-stu-id="d9579-110">When you're done, click outside of the pane to minimize the **Activities** pane.</span></span>
1. <span data-ttu-id="d9579-111">指定日期范围，然后在"用户"框中，选择要调查的用户的用户名。</span><span class="sxs-lookup"><span data-stu-id="d9579-111">Specify the date range, and then in the **Users** box, select the username for the user you want to investigate.</span></span> <span data-ttu-id="d9579-112">一次可以选择多个用户。</span><span class="sxs-lookup"><span data-stu-id="d9579-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="d9579-113">选择 **"搜索"。**</span><span class="sxs-lookup"><span data-stu-id="d9579-113">Select **Search**.</span></span> <span data-ttu-id="d9579-114">活动显示在"结果 **"下**。</span><span class="sxs-lookup"><span data-stu-id="d9579-114">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="d9579-115">若要查看详细信息，请选择一个活动，然后选择 **"详细信息"。**</span><span class="sxs-lookup"><span data-stu-id="d9579-115">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="d9579-116">有关已删除项目的其他信息（如主题行和项目被删除时的位置）将显示在 **AffectedItems** 字段中。</span><span class="sxs-lookup"><span data-stu-id="d9579-116">Additional information about the deleted item, such as the subject line and the location of the item when it was deleted, is displayed in the **AffectedItems** field.</span></span>
    > [!NOTE]
    > <span data-ttu-id="d9579-117">你无法还原使用"已删除邮件"功能审核日志项目。</span><span class="sxs-lookup"><span data-stu-id="d9579-117">You can't restore deleted items using the audit log feature.</span></span> <span data-ttu-id="d9579-118">若要还原已删除的项目，请参阅"恢复已删除项目"[或Outlook Web App。](https://go.microsoft.com/fwlink/?linkid=2103759)</span><span class="sxs-lookup"><span data-stu-id="d9579-118">To restore deleted items, see [Recover deleted items or email in Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>

<span data-ttu-id="d9579-119">若要了解更多信息，请参阅["搜索 Office 365 审核日志排查常见方案。](https://go.microsoft.com/fwlink/?linkid=2103944)</span><span class="sxs-lookup"><span data-stu-id="d9579-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>
