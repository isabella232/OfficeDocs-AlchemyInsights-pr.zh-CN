---
title: 启用存档邮箱
ms.author: markjjo
author: markjjo
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "307"
- "3100008"
ms.assetid: e1a5fab7-d3a5-4d4c-8ee2-0edf4ec9b76b
ms.openlocfilehash: 3e20eaf8dec85454ce5a67e1b21292b2a33ebb1d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47811695"
---
# <a name="enable-an-archive-mailbox"></a><span data-ttu-id="c31f3-102">启用存档邮箱</span><span class="sxs-lookup"><span data-stu-id="c31f3-102">Enable an archive mailbox</span></span>

<span data-ttu-id="c31f3-103">如果你希望我们运行自动检查以确保可以配置存档邮箱，请在此页面顶部选择 "上一步" 按钮 <--然后输入帐户的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="c31f3-103">If you want us to run automated checks to ensure an archive mailbox can be configured, select the back button <-- at the top of this page, and then enter the email address of the account.</span></span>

<span data-ttu-id="c31f3-104">Microsoft 365 中的存档邮箱 (也称为 *在线存档* 或 *就地存档*) 向用户提供额外的电子邮件存储。</span><span class="sxs-lookup"><span data-stu-id="c31f3-104">Archive mailboxes in Microsoft 365 (also called *Online Archives* or *In-Place Archives*) provide users with additional email storage.</span></span> <span data-ttu-id="c31f3-105">用户可以将项目移动或复制到其存档邮箱，并且管理员可以创建自动将项目移动到存档邮箱的存档策略。</span><span class="sxs-lookup"><span data-stu-id="c31f3-105">Users can move or copy items to their archive mailbox, and admins can create an archive policy that automatically moves items to archive mailboxes.</span></span>
  
<span data-ttu-id="c31f3-106">下面介绍了如何创建存档邮箱：</span><span class="sxs-lookup"><span data-stu-id="c31f3-106">Here's how to create an archive mailbox:</span></span>
  
1. <span data-ttu-id="c31f3-107">转到 [https://protection.office.com](https://protection.office.com)。</span><span class="sxs-lookup"><span data-stu-id="c31f3-107">Go to [https://protection.office.com](https://protection.office.com).</span></span>

2. <span data-ttu-id="c31f3-108">使用管理员帐户登录到 Microsoft 365。</span><span class="sxs-lookup"><span data-stu-id="c31f3-108">Sign in to Microsoft 365 using your admin account.</span></span>

3. <span data-ttu-id="c31f3-109">在安全合规性中心的左侧窗格中 &amp; ，选择 " **信息治理** \> **存档**"。</span><span class="sxs-lookup"><span data-stu-id="c31f3-109">In the left pane of the Security &amp; Compliance Center, select **Information governance** \> **Archive**.</span></span>

4. <span data-ttu-id="c31f3-110">选择要启用其存档邮箱的用户。</span><span class="sxs-lookup"><span data-stu-id="c31f3-110">Select the user whose archive mailbox you want to enable.</span></span>

5. <span data-ttu-id="c31f3-111">在右侧的 "详细信息" 窗格中，单击 " **启用** "，然后在警告消息中单击 **"是"** 启用存档邮箱。</span><span class="sxs-lookup"><span data-stu-id="c31f3-111">In the details pane on the right, click **Enable** and then click **Yes** in the warning message to enable the archive mailbox.</span></span>

<span data-ttu-id="c31f3-112">您还可以通过选择多个用户 (使用 **Shift** 或 **Ctrl** 键) 然后在详细信息窗格中单击 " **启用** " 来批量启用存档邮箱。</span><span class="sxs-lookup"><span data-stu-id="c31f3-112">You can also bulk-enable archive mailboxes by selecting multiple users (using the **Shift** or **Ctrl** keys) and then clicking **Enable** in the details pane.</span></span>
  
### <a name="shared-mailboxes"></a><span data-ttu-id="c31f3-113">共享邮箱</span><span class="sxs-lookup"><span data-stu-id="c31f3-113">Shared mailboxes</span></span>

<span data-ttu-id="c31f3-114">若要为共享邮箱启用存档，需要具有 Exchange Online 存档许可证的 Exchange Online 计划2许可证或 Exchange Online 计划1许可证。</span><span class="sxs-lookup"><span data-stu-id="c31f3-114">To enable the archive for a shared mailbox, an Exchange Online Plan 2 license or an Exchange Online Plan 1 license with an Exchange Online Archiving license is required.</span></span>  

<span data-ttu-id="c31f3-115">若要为共享邮箱启用存档，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="c31f3-115">To enable the archive for a shared mailbox:</span></span>

1. <span data-ttu-id="c31f3-116">转到 [Exchange 管理中心](https://outlook.office365.com/ecp) ，使用管理员帐户登录。</span><span class="sxs-lookup"><span data-stu-id="c31f3-116">Go to the [Exchange admin center](https://outlook.office365.com/ecp) and sign in using your admin account.</span></span>

2. <span data-ttu-id="c31f3-117">转到**Recipients**"  >  **共享**的收件人"。</span><span class="sxs-lookup"><span data-stu-id="c31f3-117">Go to **Recipients** > **Shared**.</span></span>

3. <span data-ttu-id="c31f3-118">选择共享邮箱。</span><span class="sxs-lookup"><span data-stu-id="c31f3-118">Select the shared mailbox.</span></span>

4. <span data-ttu-id="c31f3-119">在右侧的 "详细信息" 窗格中的 " **就地存档**" 下，单击 " **启用**"，然后单击 **"是"** 启用存档邮箱。</span><span class="sxs-lookup"><span data-stu-id="c31f3-119">In the details pane on the right, under **In-Place Archive**, click **Enable**, and then click **Yes** to enable the archive mailbox.</span></span>

<span data-ttu-id="c31f3-120">有关详细信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="c31f3-120">For more information, see:</span></span>
  
- [<span data-ttu-id="c31f3-121">启用存档邮箱</span><span class="sxs-lookup"><span data-stu-id="c31f3-121">Enable archive mailboxes</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes)

- [<span data-ttu-id="c31f3-122">设置存档和删除策略</span><span class="sxs-lookup"><span data-stu-id="c31f3-122">Set up an archive and deletion policy</span></span>](https://docs.microsoft.com//office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes)
