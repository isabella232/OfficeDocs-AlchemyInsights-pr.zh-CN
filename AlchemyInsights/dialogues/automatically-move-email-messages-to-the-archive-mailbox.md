---
title: 自动将电子邮件移动到存档邮箱
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2021
ms.locfileid: "50522356"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a><span data-ttu-id="8c4d8-102">自动将电子邮件移动到存档邮箱</span><span class="sxs-lookup"><span data-stu-id="8c4d8-102">Automatically move email messages to the archive mailbox</span></span>

<span data-ttu-id="8c4d8-103">下面是如何设置策略以将用户的旧电子邮件自动移动到存档邮箱：</span><span class="sxs-lookup"><span data-stu-id="8c4d8-103">Here's how to set up a policy to automatically move a user's old email to the archive mailbox:</span></span>

1. <span data-ttu-id="8c4d8-104">转到 [**"安全&**](https://go.microsoft.com/fwlink/p/?linkid=2077143)合规性数据管理存档"，验证存档邮箱  >    >  是否已启用用户。</span><span class="sxs-lookup"><span data-stu-id="8c4d8-104">Go to [**Security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143) > **Data governance** > **Archive** to verify an archive mailbox has been enabled for the user.</span></span> <span data-ttu-id="8c4d8-105">如果尚未启用， **请在警告框中** 单击" **启用"，** 然后单击"是"。</span><span class="sxs-lookup"><span data-stu-id="8c4d8-105">If it hasn't, click **Enable** then **Yes** in the warning box.</span></span>
2. <span data-ttu-id="8c4d8-106">转到 [**Exchange 管理中心>合规性管理>保留标记**](https://go.microsoft.com/fwlink/?linkid=2059104)。</span><span class="sxs-lookup"><span data-stu-id="8c4d8-106">Go to [**Exchange admin center > compliance management > retention tags**](https://go.microsoft.com/fwlink/?linkid=2059104).</span></span>
3. <span data-ttu-id="8c4d8-107">选择 + 图标，然后选择 **自动应用于整个邮箱**。</span><span class="sxs-lookup"><span data-stu-id="8c4d8-107">Choose the + icon then choose **automatically apply to entire mailbox**.</span></span>
4. <span data-ttu-id="8c4d8-108">为保留标记分配名称，然后选择"**移动到存档"。**</span><span class="sxs-lookup"><span data-stu-id="8c4d8-108">Assign a name to the retention tag, and choose **Move to Archive**.</span></span> <span data-ttu-id="8c4d8-109">对于保留期，输入您想要的时间，如 90 天。</span><span class="sxs-lookup"><span data-stu-id="8c4d8-109">For the retention period, enter the time you want, such as 90 days.</span></span> <span data-ttu-id="8c4d8-110">单击“**保存**”。</span><span class="sxs-lookup"><span data-stu-id="8c4d8-110">Click **Save**.</span></span>
5. <span data-ttu-id="8c4d8-111">现在创建保留策略：选择 **保留策略**，选择图标以添加新策略。</span><span class="sxs-lookup"><span data-stu-id="8c4d8-111">Now create a retention policy: choose **retention policies**, choose the icon to add a new policy.</span></span>
6. <span data-ttu-id="8c4d8-112">为保留策略分配名称，然后单击并滚动以查找并添加刚创建的保留标记。</span><span class="sxs-lookup"><span data-stu-id="8c4d8-112">Assign a name to the retention policy, then click and scroll to find and add the retention tag you just created.</span></span> <span data-ttu-id="8c4d8-113">单击“**保存**”。</span><span class="sxs-lookup"><span data-stu-id="8c4d8-113">Click **Save**.</span></span>
7. <span data-ttu-id="8c4d8-114">最后，将保留策略应用于用户的邮箱：仍在 Exchange 管理中心中，转到 **收件人**  >  **邮箱**。</span><span class="sxs-lookup"><span data-stu-id="8c4d8-114">Finally, apply the retention policy to the user's mailbox: still in the Exchange admin center, go to **recipients** > **mailboxes**.</span></span> <span data-ttu-id="8c4d8-115">选择要应用策略的所有用户，然后选择"编辑 (铅笔图标) 。 </span><span class="sxs-lookup"><span data-stu-id="8c4d8-115">Choose all the users who you want to apply the policy to, then choose **Edit** (the pencil icon).</span></span>
8. <span data-ttu-id="8c4d8-116">在对话框中，单击 **邮箱功能**。</span><span class="sxs-lookup"><span data-stu-id="8c4d8-116">In the dialog box, click **mailbox features**.</span></span> <span data-ttu-id="8c4d8-117">在 **"保留策略**"下，应用刚创建的策略> **保存**。</span><span class="sxs-lookup"><span data-stu-id="8c4d8-117">Under **Retention policy**, apply the policy you just created > **Save**.</span></span>
9. <span data-ttu-id="8c4d8-118">有关将策略应用于所有用户的说明，请参阅"将保留策略应用于[邮箱"。](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)</span><span class="sxs-lookup"><span data-stu-id="8c4d8-118">For instructions for applying the policy to all users, see [Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span></span>
