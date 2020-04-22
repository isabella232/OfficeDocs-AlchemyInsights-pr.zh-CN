---
title: Outlook 桌面撤回或替换电子邮件
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: d64332778f9132aff6a9660bb0d522f4e16b753c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687500"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="7332d-102">撤回或替换 Outlook 电子邮件</span><span class="sxs-lookup"><span data-stu-id="7332d-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="7332d-103">作为管理员，你可以**使用 PowerShell 代表用户撤回邮件**。</span><span class="sxs-lookup"><span data-stu-id="7332d-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="7332d-104">无法从管理中心撤回邮件。</span><span class="sxs-lookup"><span data-stu-id="7332d-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="7332d-105">您**只能撤回发送给组织中的人员的邮件**。</span><span class="sxs-lookup"><span data-stu-id="7332d-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="7332d-106">例如，如果邮件发送到 Gmail 地址，则无法撤回它。</span><span class="sxs-lookup"><span data-stu-id="7332d-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="7332d-107">**只能撤回从电脑上的 Outlook 2016 发送的邮件**。</span><span class="sxs-lookup"><span data-stu-id="7332d-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="7332d-108">如果用户使用 Outlook for Mac 或 web 上的 Outlook 发送邮件，则无法撤回它。</span><span class="sxs-lookup"><span data-stu-id="7332d-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="7332d-109">若要撤回或替换电子邮件，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="7332d-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="7332d-110">在 Outlook 窗口左侧的文件夹窗格中，选择 "已发送邮件" 文件夹。</span><span class="sxs-lookup"><span data-stu-id="7332d-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="7332d-111">双击要撤回的邮件以将其打开。</span><span class="sxs-lookup"><span data-stu-id="7332d-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="7332d-112">选择 "**邮件**" 选项卡，然后选择 "**操作** > **撤回此邮件**"。</span><span class="sxs-lookup"><span data-stu-id="7332d-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="7332d-113">选择 "**删除此邮件的未读副本**" 或 "**删除未读副本并将其替换为新邮件**"，然后选择 **"确定"**。</span><span class="sxs-lookup"><span data-stu-id="7332d-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="7332d-114">如果要发送替换邮件，请撰写邮件，然后选择 "**发送**"。</span><span class="sxs-lookup"><span data-stu-id="7332d-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="7332d-115">邮件撤回的成功或失败取决于收件人在 Outlook 中的设置。</span><span class="sxs-lookup"><span data-stu-id="7332d-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="7332d-116">有关检查召回的步骤，请参阅[本文](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)。</span><span class="sxs-lookup"><span data-stu-id="7332d-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="7332d-117">在组织中搜索和删除电子邮件</span><span class="sxs-lookup"><span data-stu-id="7332d-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="7332d-118">如果您不是全局管理员，则必须将您的帐户添加到电子数据展示管理器角色或合规性搜索管理角色中，才能搜索邮件。</span><span class="sxs-lookup"><span data-stu-id="7332d-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="7332d-119">若要删除邮件，您需要加入组织管理角色组或搜索和清除管理角色。</span><span class="sxs-lookup"><span data-stu-id="7332d-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="7332d-120">在[安全与合规中心](https://go.microsoft.com/fwlink/?linkid=2083731)中分配这些角色的权限。</span><span class="sxs-lookup"><span data-stu-id="7332d-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="7332d-121">[创建内容搜索](https://docs.microsoft.com/office365/securitycompliance/content-search)以查找要删除的邮件。</span><span class="sxs-lookup"><span data-stu-id="7332d-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="7332d-122">[连接到安全与合规中心 PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)。</span><span class="sxs-lookup"><span data-stu-id="7332d-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="7332d-123">如果使用的是多重身份验证，请参阅[使用多重身份验证连接到 Microsoft 365 安全与合规中心 PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)。</span><span class="sxs-lookup"><span data-stu-id="7332d-123">If you're using multi-factor authentication, see [Connect to Microsoft 365 security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>