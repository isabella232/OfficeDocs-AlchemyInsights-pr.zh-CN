---
title: 确定审核日志中邮箱的外部电子邮件转发
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 156fd0044cdc42230ace0a5db16f49af572bb6fa
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716450"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="41030-102">确定何时在邮箱上配置了外部电子邮件转发</span><span class="sxs-lookup"><span data-stu-id="41030-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="41030-103">当 Microsoft 365 用户在邮箱上配置外部电子邮件转发时，该活动将作为**设置邮箱**cmdlet 的一部分进行审核。</span><span class="sxs-lookup"><span data-stu-id="41030-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="41030-104">您可以使用安全 & 合规性中心中的 "审核日志搜索" 查看活动。</span><span class="sxs-lookup"><span data-stu-id="41030-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="41030-105">登录到[Microsoft 365 安全 & 合规性中心](https://protection.office.com/)。</span><span class="sxs-lookup"><span data-stu-id="41030-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="41030-106">转到 "**搜索** > **审核日志搜索**" 页。</span><span class="sxs-lookup"><span data-stu-id="41030-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="41030-107">在 "**开始日期**" 和 "**结束日期**" 字段中选择日期范围。</span><span class="sxs-lookup"><span data-stu-id="41030-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="41030-108">无需指定用户名。</span><span class="sxs-lookup"><span data-stu-id="41030-108">You don't need to specify a username.</span></span> <span data-ttu-id="41030-109">验证 "**活动**" 字段是否设置为**显示所有活动的结果**。</span><span class="sxs-lookup"><span data-stu-id="41030-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="41030-110">单击"搜索"。</span><span class="sxs-lookup"><span data-stu-id="41030-110">Click **Search**.</span></span>

<span data-ttu-id="41030-111">在结果中，单击 "活动筛选器" 框中的 "**筛选结果**并键入 '**设置 '-邮箱**"。</span><span class="sxs-lookup"><span data-stu-id="41030-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="41030-112">在结果中选择一个审核记录。</span><span class="sxs-lookup"><span data-stu-id="41030-112">Select an audit record in the results.</span></span> <span data-ttu-id="41030-113">在 "**详细**信息" 浮出控件中，单击 "**详细信息**"。</span><span class="sxs-lookup"><span data-stu-id="41030-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="41030-114">您必须查看每个审核记录的详细信息，以确定该活动是否与电子邮件转发相关。</span><span class="sxs-lookup"><span data-stu-id="41030-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="41030-115">**ObjectId**：已修改的邮箱的别名值。</span><span class="sxs-lookup"><span data-stu-id="41030-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="41030-116">**参数**： _ForwardingSmtpAddress_表示目标电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="41030-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="41030-117">**UserId**：在**ObjectId**字段中的邮箱上配置电子邮件转发的用户。</span><span class="sxs-lookup"><span data-stu-id="41030-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="41030-118">有关详细信息，请参阅[确定为邮箱设置电子邮件转发](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox)。</span><span class="sxs-lookup"><span data-stu-id="41030-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
