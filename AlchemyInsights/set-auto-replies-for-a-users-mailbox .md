---
title: 设置用户邮箱的自动答复
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: e3cc01298c10fd3ba21327a7fb5cc5396d0ad74d
ms.sourcegitcommit: 23e5b94f1758bfe202008384e300b81816975375
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43506422"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="2dec8-102">设置用户邮箱的自动答复</span><span class="sxs-lookup"><span data-stu-id="2dec8-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="2dec8-103">**方法 1**</span><span class="sxs-lookup"><span data-stu-id="2dec8-103">**Method 1**</span></span>

1. <span data-ttu-id="2dec8-104">登录 Office 365 门户。</span><span class="sxs-lookup"><span data-stu-id="2dec8-104">Sign in to the Office 365 portal.</span></span>

2. <span data-ttu-id="2dec8-105">转到 **“用户”>“活动用户”**（或如果在共享邮箱上进行设置，则转到 **“组”>“共享邮箱”**）。</span><span class="sxs-lookup"><span data-stu-id="2dec8-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="2dec8-106">选择具有 Microsoft Exchange 邮箱的用户。</span><span class="sxs-lookup"><span data-stu-id="2dec8-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="2dec8-107">在右侧的弹出菜单上，转到 **“邮件设置”>“自动答复”**（如果是共享邮箱，只需在弹出菜单上单击“**自动答复**”）。</span><span class="sxs-lookup"><span data-stu-id="2dec8-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="2dec8-108">**方法 2**</span><span class="sxs-lookup"><span data-stu-id="2dec8-108">**Method 2**</span></span>

1. <span data-ttu-id="2dec8-109">使用管理员凭据登录到 Office 365 管理门户。</span><span class="sxs-lookup"><span data-stu-id="2dec8-109">Sign in to the Office 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="2dec8-110">展开“**管理中心**”，然后单击“**Exchange**”。</span><span class="sxs-lookup"><span data-stu-id="2dec8-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="2dec8-111">单击右上角的图片，单击“**其他用户**”，然后选择要更改的用户邮箱。</span><span class="sxs-lookup"><span data-stu-id="2dec8-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="2dec8-112">在左侧，选择“**选项**”，单击“**组织电子邮件**”，然后单击“**自动答复**”。</span><span class="sxs-lookup"><span data-stu-id="2dec8-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="2dec8-113">**方法 3**</span><span class="sxs-lookup"><span data-stu-id="2dec8-113">**Method 3**</span></span>

<span data-ttu-id="2dec8-114">在 Exchange Online PowerShell 中运行以下 cmdlet：</span><span class="sxs-lookup"><span data-stu-id="2dec8-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="2dec8-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="2dec8-115">PowerShellCopy</span></span>

    Set-MailboxAutoReplyConfiguration

<span data-ttu-id="2dec8-116">有关此 cmdlet 的详细信息，请参阅 [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration)。</span><span class="sxs-lookup"><span data-stu-id="2dec8-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
