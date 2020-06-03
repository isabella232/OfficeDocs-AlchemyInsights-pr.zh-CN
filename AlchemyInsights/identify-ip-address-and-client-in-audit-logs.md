---
title: 在审核日志中标识 IP 地址和客户端
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 80b652eb65612093252dee226a19ec74bc035faa
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508906"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="c82f2-102">在审核日志中标识 IP 地址和客户端</span><span class="sxs-lookup"><span data-stu-id="c82f2-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="c82f2-103">与 Microsoft 365 用户或管理员的活动对应的 IP 地址显示在审核日志中。</span><span class="sxs-lookup"><span data-stu-id="c82f2-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="c82f2-104">还记录客户端信息。</span><span class="sxs-lookup"><span data-stu-id="c82f2-104">The client information is also logged.</span></span> <span data-ttu-id="c82f2-105">以下是确定此类信息的步骤</span><span class="sxs-lookup"><span data-stu-id="c82f2-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="c82f2-106">登录到[Microsoft 365 安全 & 合规性中心](https://protection.office.com/)。</span><span class="sxs-lookup"><span data-stu-id="c82f2-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="c82f2-107">转到 "**搜索**  >  **审核日志搜索**" 页。</span><span class="sxs-lookup"><span data-stu-id="c82f2-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="c82f2-108">如果你对特定活动感兴趣，请从 "**活动**" 列表中选择该活动。</span><span class="sxs-lookup"><span data-stu-id="c82f2-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="c82f2-109">如果不是，则将返回选定用户的所有活动（默认设置）。</span><span class="sxs-lookup"><span data-stu-id="c82f2-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="c82f2-110">**注意**：某些活动可能在 "**活动**" 菜单中不可用;但是，如果选择 "**显示所有活动的结果**"，则将返回这些审核项目（默认设置）。</span><span class="sxs-lookup"><span data-stu-id="c82f2-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="c82f2-111">在 "**用户**" 字段中指定用户名，为活动选择适当的日期范围，然后单击 "**搜索**"。</span><span class="sxs-lookup"><span data-stu-id="c82f2-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="c82f2-112">在结果中，可以在 "结果" 窗格中看到该活动的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="c82f2-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="c82f2-113">选择 "审核记录" 可查看 "**详细**信息" 浮出控件中的详细信息（例如，客户端、执行操作的用户等）。</span><span class="sxs-lookup"><span data-stu-id="c82f2-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="c82f2-114">有关详细信息，请参阅[查找用于访问已损坏帐户的计算机的 IP 地址](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account)。</span><span class="sxs-lookup"><span data-stu-id="c82f2-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
