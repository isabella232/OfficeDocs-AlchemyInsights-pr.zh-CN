---
title: 创建电子邮件全部捕获
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712976"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="8a041-102">创建电子邮件全部捕获</span><span class="sxs-lookup"><span data-stu-id="8a041-102">Create an email catch all</span></span>

<span data-ttu-id="8a041-103">强烈建议不要使用全部捕获。</span><span class="sxs-lookup"><span data-stu-id="8a041-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="8a041-104">更好的方法是，让发件人向发件人告知其邮件无法按寻址方式传递，这样他们就可以采取措施。</span><span class="sxs-lookup"><span data-stu-id="8a041-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="8a041-105">您还可以将受监视的邮箱限制为仅捕获以前有效的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="8a041-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="8a041-106">任何捕获所有邮箱都将收到大量垃圾邮件，并且最终可能会填写（如果未受到严密监控）。</span><span class="sxs-lookup"><span data-stu-id="8a041-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="8a041-107"> (有接收限制。 ) </span><span class="sxs-lookup"><span data-stu-id="8a041-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="8a041-108">如果你决定继续，请按照以下步骤操作：</span><span class="sxs-lookup"><span data-stu-id="8a041-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="8a041-109">创建动态通讯组，& 包括 "所有收件人类型"。</span><span class="sxs-lookup"><span data-stu-id="8a041-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="8a041-110">创建专用邮箱来捕获电子邮件，例如，catchall@domain.com。</span><span class="sxs-lookup"><span data-stu-id="8a041-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="8a041-111">对于特定域，将 DomainType 设置为 "InternalRelay"。</span><span class="sxs-lookup"><span data-stu-id="8a041-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="8a041-112">如果稍后删除 "全部捕获"，请务必将域重新设置为权威。</span><span class="sxs-lookup"><span data-stu-id="8a041-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="8a041-113">创建邮件流传输规则，如下所示：</span><span class="sxs-lookup"><span data-stu-id="8a041-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="8a041-114">如果发件人是 "组织外部"</span><span class="sxs-lookup"><span data-stu-id="8a041-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="8a041-115">将邮件重定向到 Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="8a041-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="8a041-116">除非收件人是 allusers@domain.com 的成员 (通讯组包含所有成员) </span><span class="sxs-lookup"><span data-stu-id="8a041-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="8a041-117">确保新邮箱已添加到动态通讯组中</span><span class="sxs-lookup"><span data-stu-id="8a041-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
