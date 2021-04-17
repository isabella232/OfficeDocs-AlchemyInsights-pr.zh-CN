---
title: 创建电子邮件捕获全部
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816190"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="2ba0d-102">创建电子邮件捕获全部</span><span class="sxs-lookup"><span data-stu-id="2ba0d-102">Create an email catch all</span></span>

<span data-ttu-id="2ba0d-103">强烈建议不要使用 catch all。</span><span class="sxs-lookup"><span data-stu-id="2ba0d-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="2ba0d-104">最好向发件人提供退回邮件，让发件人知道他们的邮件无法以地址方式传递，以便可以采取措施。</span><span class="sxs-lookup"><span data-stu-id="2ba0d-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="2ba0d-105">您还可以将受监视的邮箱限制为仅捕获以前有效的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="2ba0d-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="2ba0d-106">任何捕获所有邮箱都将收到大量垃圾邮件，如果未受到密切监视，最终可能会填充这些垃圾邮件。</span><span class="sxs-lookup"><span data-stu-id="2ba0d-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="2ba0d-107"> (有接收限制。) </span><span class="sxs-lookup"><span data-stu-id="2ba0d-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="2ba0d-108">如果您决定继续，请按照以下步骤操作：</span><span class="sxs-lookup"><span data-stu-id="2ba0d-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="2ba0d-109">创建包含"所有&"的动态通讯组。</span><span class="sxs-lookup"><span data-stu-id="2ba0d-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="2ba0d-110">创建专用邮箱以捕获电子邮件，例如，catchall@domain.com。</span><span class="sxs-lookup"><span data-stu-id="2ba0d-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="2ba0d-111">对于特定域，将 DomainType 设置为"InternalRelay"。</span><span class="sxs-lookup"><span data-stu-id="2ba0d-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="2ba0d-112">如果稍后删除 catch all，请确保将域设置回"权威"。</span><span class="sxs-lookup"><span data-stu-id="2ba0d-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="2ba0d-113">创建邮件流传输规则，如下所示：</span><span class="sxs-lookup"><span data-stu-id="2ba0d-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="2ba0d-114">如果发件人为"组织外部"</span><span class="sxs-lookup"><span data-stu-id="2ba0d-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="2ba0d-115">将邮件重定向到 Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="2ba0d-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="2ba0d-116">除非收件人是通讯组的成员 allusers@domain.com (通讯组包含所有) </span><span class="sxs-lookup"><span data-stu-id="2ba0d-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="2ba0d-117">确保验证是否将新邮箱添加到动态通讯组</span><span class="sxs-lookup"><span data-stu-id="2ba0d-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
