---
title: 撤回或替换电子邮件
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353496"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a><span data-ttu-id="0d087-102">在 Microsoft 365 中撤回或替换电子邮件</span><span class="sxs-lookup"><span data-stu-id="0d087-102">Recall or replace an email message in Microsoft 365</span></span>

- <span data-ttu-id="0d087-103">您 **只能撤回发送给组织中的人员的邮件**。</span><span class="sxs-lookup"><span data-stu-id="0d087-103">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="0d087-104">例如，如果邮件发送到 Gmail 地址，则无法撤回它。</span><span class="sxs-lookup"><span data-stu-id="0d087-104">For example, if the message was sent to a Gmail address, you can't recall it.</span></span>
- <span data-ttu-id="0d087-105">您 **只能撤回从 Outlook 为电脑发送的邮件**。</span><span class="sxs-lookup"><span data-stu-id="0d087-105">You can **only recall messages sent from Outlook for the PC**.</span></span> <span data-ttu-id="0d087-106">如果用户使用 Outlook for Mac 或 web 上的 Outlook 发送邮件，则无法撤回它。</span><span class="sxs-lookup"><span data-stu-id="0d087-106">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>
- <span data-ttu-id="0d087-107">作为租户管理员，你可以 **使用 PowerShell (代表用户撤回邮件** 。有关详细信息，请参阅： [Search For and delete email messages](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)) 。</span><span class="sxs-lookup"><span data-stu-id="0d087-107">As a tenant administrator, you can **recall messages on behalf of users by using PowerShell** (For more information, see: [Search for and delete email messages](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span></span>
- <span data-ttu-id="0d087-108">无法从管理中心撤回邮件。</span><span class="sxs-lookup"><span data-stu-id="0d087-108">You can't recall messages from the admin center.</span></span> <span data-ttu-id="0d087-109">向下滚动到 "搜索组织中的电子邮件并删除电子邮件"，了解详细信息。</span><span class="sxs-lookup"><span data-stu-id="0d087-109">Scroll down to "Search for and delete email messages in your organization" for more information.</span></span>

<span data-ttu-id="0d087-110">**撤回或替换您发送的电子邮件**</span><span class="sxs-lookup"><span data-stu-id="0d087-110">**Recall or replace an email message that you sent**</span></span>

1. <span data-ttu-id="0d087-111">在 Outlook 窗口左侧的文件夹窗格中，选择 "已发送邮件" 文件夹。</span><span class="sxs-lookup"><span data-stu-id="0d087-111">In the folder pane on the left of the Outlook window, choose the Sent Items folder.</span></span>
2. <span data-ttu-id="0d087-112">打开要撤回的邮件。</span><span class="sxs-lookup"><span data-stu-id="0d087-112">Open the message that you want to recall.</span></span> <span data-ttu-id="0d087-113">您必须双击才能打开邮件。</span><span class="sxs-lookup"><span data-stu-id="0d087-113">You must double-click to open the message.</span></span> <span data-ttu-id="0d087-114">如果选择邮件使其显示在阅读窗格中，则不会允许您撤回邮件。</span><span class="sxs-lookup"><span data-stu-id="0d087-114">Selecting the message so it appears in the reading pane won't allow you to recall the message.</span></span>
3. <span data-ttu-id="0d087-115">从 "邮件" 选项卡中，选择 "**操作**  >  **撤回此邮件**"。</span><span class="sxs-lookup"><span data-stu-id="0d087-115">From the Message tab, select **Actions** > **Recall This Message**.</span></span>
4. <span data-ttu-id="0d087-116">选择 " **删除此邮件的未读副本** " 或 " **删除未读副本并将其替换为新邮件**"，然后选择 **"确定"**。</span><span class="sxs-lookup"><span data-stu-id="0d087-116">Choose **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, then select **OK**.</span></span>
5. <span data-ttu-id="0d087-117">如果要发送替换邮件，请撰写邮件，然后选择 " **发送**"。</span><span class="sxs-lookup"><span data-stu-id="0d087-117">If you're sending a replacement message, compose the message, then select **Send**.</span></span>
6. <span data-ttu-id="0d087-118">邮件撤回的成功或失败取决于收件人在 Outlook 中的设置。</span><span class="sxs-lookup"><span data-stu-id="0d087-118">The success or failure of a message recall depends on the recipients' settings in Outlook.</span></span>

<span data-ttu-id="0d087-119">有关详细信息，包括如何检查撤回，请参阅 [撤回或 replace 您发送的电子](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)邮件。</span><span class="sxs-lookup"><span data-stu-id="0d087-119">For more information, including how to check on the recall, see [Recall or replace an email message that you sent](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="0d087-120">**_若要在组织中搜索和删除电子邮件_**，您是全局管理员的最简单方法。如果您不是全局管理员，则必须将您的帐户添加到电子数据展示管理器角色组或合规性搜索管理角色。</span><span class="sxs-lookup"><span data-stu-id="0d087-120">**_To search for and delete email messages in your organization_**, it's easiest if you're a global admin. If you're not a global admin, your account must be added to the eDiscovery Manager role group, or to the Compliance Search management role.</span></span> <span data-ttu-id="0d087-121">若要删除邮件，您需要加入组织管理角色组或搜索和清除管理角色。</span><span class="sxs-lookup"><span data-stu-id="0d087-121">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="0d087-122">对这些角色的权限是在 [安全 & 合规中心](https://protection.office.com/)中分配的。</span><span class="sxs-lookup"><span data-stu-id="0d087-122">Permissions to these roles are assigned in the [Security & compliance center](https://protection.office.com/).</span></span>

1. <span data-ttu-id="0d087-123">[创建内容搜索](https://docs.microsoft.com/microsoft-365/compliance/content-search) 以查找要删除的邮件。</span><span class="sxs-lookup"><span data-stu-id="0d087-123">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
2. <span data-ttu-id="0d087-124">[连接到安全与合规中心 PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)。</span><span class="sxs-lookup"><span data-stu-id="0d087-124">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span>

<span data-ttu-id="0d087-125">如果你正在使用 MFA (多重身份验证) ，请参阅 [使用多重身份验证连接到 Microsoft 365 Security & 合规性中心 PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)。</span><span class="sxs-lookup"><span data-stu-id="0d087-125">If you're using MFA (multi-factor authentication), see [Connect to Microsoft 365 Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span></span>
