---
title: 确定审核日志中的收件箱规则活动
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1368
ms.assetid: ''
ms.openlocfilehash: f130846dd24cef81177934aa2a200c1056172d3f
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/07/2019
ms.locfileid: "34755028"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="8cfbd-102">确定审核日志中的收件箱规则活动</span><span class="sxs-lookup"><span data-stu-id="8cfbd-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="8cfbd-103">您可以使用安全 & 合规性中心中的审核日志搜索来查看收件箱规则事件 (创建、修改和删除收件箱规则)。</span><span class="sxs-lookup"><span data-stu-id="8cfbd-103">You can use audit log search in the Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="8cfbd-104">登录到[Office 365 安全 & 合规中心](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="8cfbd-104">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="8cfbd-105">单击 "**搜索和调查**", 然后选择 "**审核日志搜索**"。</span><span class="sxs-lookup"><span data-stu-id="8cfbd-105">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="8cfbd-106">在 "**开始日期**" 和 "**结束日期**" 字段中选择日期范围。</span><span class="sxs-lookup"><span data-stu-id="8cfbd-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="8cfbd-107">在 " **Exchange 邮箱活动**" 下, 验证 "**活动**" 字段是否设置为**new-inboxrule "创建/修改/启用/禁用收件箱规则"**。</span><span class="sxs-lookup"><span data-stu-id="8cfbd-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="8cfbd-108">单击"搜索"。</span><span class="sxs-lookup"><span data-stu-id="8cfbd-108">Click **Search**.</span></span>

<span data-ttu-id="8cfbd-109">在结果中, 选择一个审核记录。</span><span class="sxs-lookup"><span data-stu-id="8cfbd-109">In the results, select an audit record.</span></span> <span data-ttu-id="8cfbd-110">在 "详细信息" 浮出控件中, 单击 "**详细信息**"。</span><span class="sxs-lookup"><span data-stu-id="8cfbd-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="8cfbd-111">有关收件箱规则设置的信息将显示在 "**参数**" 字段中。</span><span class="sxs-lookup"><span data-stu-id="8cfbd-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="8cfbd-112">有关详细信息, 请参阅[确定用户是否已创建收件箱规则](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="8cfbd-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
