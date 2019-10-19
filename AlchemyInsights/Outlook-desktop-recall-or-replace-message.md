---
title: Outlook 桌面撤回或替换电子邮件
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 3d3a6c253317137b7069a978b907c97d61bf7313
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2019
ms.locfileid: "36496101"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="b48ee-102">撤回或替换 Outlook 电子邮件</span><span class="sxs-lookup"><span data-stu-id="b48ee-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="b48ee-103">作为管理员，你可以**使用 PowerShell 代表用户撤回邮件**。</span><span class="sxs-lookup"><span data-stu-id="b48ee-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="b48ee-104">无法从管理中心撤回邮件。</span><span class="sxs-lookup"><span data-stu-id="b48ee-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="b48ee-105">您**只能撤回发送给组织中的人员的邮件**。</span><span class="sxs-lookup"><span data-stu-id="b48ee-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="b48ee-106">例如，如果邮件发送到 Gmail 地址，则无法撤回它。</span><span class="sxs-lookup"><span data-stu-id="b48ee-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="b48ee-107">**只能撤回从电脑上的 Outlook 2016 发送的邮件**。</span><span class="sxs-lookup"><span data-stu-id="b48ee-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="b48ee-108">如果用户使用 Outlook for Mac 或 web 上的 Outlook 发送邮件，则无法撤回它。</span><span class="sxs-lookup"><span data-stu-id="b48ee-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="b48ee-109">若要撤回或替换电子邮件，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="b48ee-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="b48ee-110">在 Outlook 窗口左侧的文件夹窗格中，选择 "已发送邮件" 文件夹。</span><span class="sxs-lookup"><span data-stu-id="b48ee-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="b48ee-111">双击要撤回的邮件以将其打开。</span><span class="sxs-lookup"><span data-stu-id="b48ee-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="b48ee-112">选择 "**邮件**" 选项卡，然后选择 "**操作** > **撤回此邮件**"。</span><span class="sxs-lookup"><span data-stu-id="b48ee-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="b48ee-113">选择 "**删除此邮件的未读副本**" 或 "**删除未读副本并将其替换为新邮件**"，然后选择 **"确定"**。</span><span class="sxs-lookup"><span data-stu-id="b48ee-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="b48ee-114">如果要发送替换邮件，请撰写邮件，然后选择 "**发送**"。</span><span class="sxs-lookup"><span data-stu-id="b48ee-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="b48ee-115">邮件撤回的成功或失败取决于收件人在 Outlook 中的设置。</span><span class="sxs-lookup"><span data-stu-id="b48ee-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="b48ee-116">有关检查召回的步骤，请参阅[本文](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)。</span><span class="sxs-lookup"><span data-stu-id="b48ee-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="b48ee-117">在组织中搜索和删除电子邮件</span><span class="sxs-lookup"><span data-stu-id="b48ee-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="b48ee-118">如果您不是全局管理员，则必须将您的帐户添加到电子数据展示管理器角色或合规性搜索管理角色中，才能搜索邮件。</span><span class="sxs-lookup"><span data-stu-id="b48ee-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="b48ee-119">若要删除邮件，您需要加入组织管理角色组或搜索和清除管理角色。</span><span class="sxs-lookup"><span data-stu-id="b48ee-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="b48ee-120">在[安全与合规中心](https://go.microsoft.com/fwlink/?linkid=2083731)中分配这些角色的权限。</span><span class="sxs-lookup"><span data-stu-id="b48ee-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="b48ee-121">[创建内容搜索](https://docs.microsoft.com/office365/securitycompliance/content-search)以查找要删除的邮件。</span><span class="sxs-lookup"><span data-stu-id="b48ee-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="b48ee-122">[连接到安全与合规中心 PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)。</span><span class="sxs-lookup"><span data-stu-id="b48ee-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="b48ee-123">如果使用的是多重身份验证，请参阅[使用多重身份验证连接到 Office 365 安全与合规中心 PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)。</span><span class="sxs-lookup"><span data-stu-id="b48ee-123">If you're using multi-factor authentication, see [Connect to Office 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>