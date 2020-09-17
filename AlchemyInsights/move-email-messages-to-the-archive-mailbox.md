---
title: 将电子邮件移动到存档邮箱
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799770"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="be367-102">将电子邮件移动到存档邮箱</span><span class="sxs-lookup"><span data-stu-id="be367-102">Move email to the archive mailbox</span></span>

<span data-ttu-id="be367-103">如果您希望我们为下面提到的设置运行自动检查，请在此页面顶部选择 "上一步" 按钮 <--然后输入在将电子邮件移动到其存档邮箱时遇到问题的用户的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="be367-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems moving email to their archive mailbox.</span></span>

1. <span data-ttu-id="be367-104">确认已启用 **存档邮箱** 。</span><span class="sxs-lookup"><span data-stu-id="be367-104">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="be367-105">如果不是，请使用 [本文](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) 中的步骤启用存档邮箱。</span><span class="sxs-lookup"><span data-stu-id="be367-105">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="be367-106">若要将邮件自动存档到存档邮箱，必须将包含 " **移动到存档** " 操作的保留标记设置为 "已 **自动应用于整个邮箱 (默认) 标记**。</span><span class="sxs-lookup"><span data-stu-id="be367-106">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="be367-107">使用此处的步骤创建标记： [存档默认标记](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag)。</span><span class="sxs-lookup"><span data-stu-id="be367-107">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="be367-108">接下来，将 **存档** 标记添加到保留策略中。</span><span class="sxs-lookup"><span data-stu-id="be367-108">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="be367-109">在 Exchange 管理中心中，选择 " **保留策略** " > 将 " **移动到存档" 标记** 添加到策略中 > **保存**。</span><span class="sxs-lookup"><span data-stu-id="be367-109">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="be367-110">现在， [将保留策略分配](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) 给特定用户的邮箱。</span><span class="sxs-lookup"><span data-stu-id="be367-110">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="be367-111">同一策略将同时应用于 **主** 邮箱和 **存档** 邮箱。</span><span class="sxs-lookup"><span data-stu-id="be367-111">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="be367-112">可能需要强制托管文件夹助理 (MFA) 运行新设置并将其应用于用户邮箱。</span><span class="sxs-lookup"><span data-stu-id="be367-112">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="be367-113">在 [连接到 EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) 时运行以下命令，以启动特定邮箱的托管文件夹助理：</span><span class="sxs-lookup"><span data-stu-id="be367-113">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="be367-114">启动-Start-managedfolderassistant-Identity <name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="be367-114">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="be367-115">有关设置存档策略的详细信息，请参阅 [设置邮箱的存档和删除策略](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)。</span><span class="sxs-lookup"><span data-stu-id="be367-115">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  