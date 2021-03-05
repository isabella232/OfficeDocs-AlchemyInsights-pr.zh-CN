---
title: 在邮件中查找 IP 审核日志
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
ms.openlocfilehash: 7a01aa3cc0d875e6534435f3e8f90a24f2832dc3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464504"
---
# <a name="find-the-ip-address-in-audit-log"></a><span data-ttu-id="fcd10-102">在邮件中查找 IP 审核日志</span><span class="sxs-lookup"><span data-stu-id="fcd10-102">Find the IP address in audit log</span></span>

1. <span data-ttu-id="fcd10-103">与用户或管理员执行的活动对应的 IP 地址显示在审核日志中。</span><span class="sxs-lookup"><span data-stu-id="fcd10-103">The IP address that corresponds to an activity performed by a user or administrator is shown in the audit logs.</span></span> <span data-ttu-id="fcd10-104">还会记录客户端信息。</span><span class="sxs-lookup"><span data-stu-id="fcd10-104">The client information is also logged.</span></span> <span data-ttu-id="fcd10-105">下面是如何标识 IP 地址的：</span><span class="sxs-lookup"><span data-stu-id="fcd10-105">Here's how to identify the IP address:</span></span>

1. <span data-ttu-id="fcd10-106">转到 [Office 365 安全&合规中心](https://go.microsoft.com/fwlink/p/?linkid=2077143)。</span><span class="sxs-lookup"><span data-stu-id="fcd10-106">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="fcd10-107">选择 **"搜索**  >  **[审核日志搜索"。](https://go.microsoft.com/fwlink/?linkid=2103759)**</span><span class="sxs-lookup"><span data-stu-id="fcd10-107">Select **Search** > **[Audit log search](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="fcd10-108">如果看到需要启用审核的通知，请继续，然后现在将其打开。</span><span class="sxs-lookup"><span data-stu-id="fcd10-108">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="fcd10-109">如果未启用此功能，搜索结果将无法从以前的日期拉取数据。</span><span class="sxs-lookup"><span data-stu-id="fcd10-109">If this feature isn't enabled, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="fcd10-110">如果您对特定活动感兴趣，请从"活动" **列表中选择它;** 否则，默认情况下，将为所选用户返回所有活动。</span><span class="sxs-lookup"><span data-stu-id="fcd10-110">If you're interested in a specific activity, select it from the **Activities** list; otherwise, by default, all activities will be returned for the selected user.</span></span> <span data-ttu-id="fcd10-111">请注意，某些活动可能无法从"活动"菜单中 **选择**;但是，如果在默认设置下选中"显示所有活动的结果"， (将返回) 。</span><span class="sxs-lookup"><span data-stu-id="fcd10-111">Note that certain activities might not be available for selection from the **Activities** menu; however, those audit items will be returned if **Show results for all activities** is selected (default setting).</span></span>
1. <span data-ttu-id="fcd10-112">指定日期范围，在"用户" **字段中，** 选择要调查的用户的用户名。</span><span class="sxs-lookup"><span data-stu-id="fcd10-112">Specify the date range, and in the **Users** field, select the username for the user you want to investigate.</span></span>
1. <span data-ttu-id="fcd10-113">选择 **"搜索"。**</span><span class="sxs-lookup"><span data-stu-id="fcd10-113">Select **Search**.</span></span> <span data-ttu-id="fcd10-114">活动显示在"结果 **"下**。</span><span class="sxs-lookup"><span data-stu-id="fcd10-114">The activities appear under **Results**.</span></span> <span data-ttu-id="fcd10-115">你可以看到每个活动的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="fcd10-115">You can see the IP address for each activity.</span></span>
1. <span data-ttu-id="fcd10-116">若要查看详细信息，请选择一个活动，然后选择 **"详细信息"。**</span><span class="sxs-lookup"><span data-stu-id="fcd10-116">To view details, select an activity, and then select **More Information**.</span></span>

<span data-ttu-id="fcd10-117">若要了解更多信息，请参阅"[搜索 Office 365 审核日志排查常见方案。](https://go.microsoft.com/fwlink/?linkid=2103944)</span><span class="sxs-lookup"><span data-stu-id="fcd10-117">To learn more, see Search the [Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>