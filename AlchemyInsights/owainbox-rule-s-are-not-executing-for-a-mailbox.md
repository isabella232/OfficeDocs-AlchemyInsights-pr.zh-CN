---
title: 1332 OWA-收件箱规则未对邮箱执行
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1332
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 9e782faa59bb9a16c271f7c46c79635961e88aed
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/22/2019
ms.locfileid: "30784332"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="66e90-102">收件箱规则不能按预期工作</span><span class="sxs-lookup"><span data-stu-id="66e90-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="66e90-103">验证以下设置:</span><span class="sxs-lookup"><span data-stu-id="66e90-103">Verify the following settings:</span></span>
  
- <span data-ttu-id="66e90-104">可以基于收件箱规则自动重定向、转发或答复邮件一次。</span><span class="sxs-lookup"><span data-stu-id="66e90-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="66e90-105">重定向规则 (收件箱规则或邮件流规则, 也称为传输规则) 最多可以向邮件中添加10个转发收件人。</span><span class="sxs-lookup"><span data-stu-id="66e90-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="66e90-106">有关详细信息, 请参阅[日记、Transport 和收件箱规则限制](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)。</span><span class="sxs-lookup"><span data-stu-id="66e90-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>
    
- <span data-ttu-id="66e90-107">收件箱规则在备用日记邮箱中不起作用。</span><span class="sxs-lookup"><span data-stu-id="66e90-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="66e90-108">有关备用日记邮箱的详细信息, 请参阅[备用日记邮箱](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)。</span><span class="sxs-lookup"><span data-stu-id="66e90-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>
    
<span data-ttu-id="66e90-109">若要解决这些问题, 请参阅[KB 2829319](https://support.microsoft.com/kb/2829319)。</span><span class="sxs-lookup"><span data-stu-id="66e90-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>
  
<span data-ttu-id="66e90-110">如果未应用以前的问题, 请在将问题升级到 Microsoft 支持之前运行 "收件箱规则诊断报告":</span><span class="sxs-lookup"><span data-stu-id="66e90-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>
  
1. <span data-ttu-id="66e90-111">打开 web 上的 Outlook 中的邮箱, 然后单击 "**设置** \> **选项** \> **组织电子邮件** \> **收件箱规则**"。</span><span class="sxs-lookup"><span data-stu-id="66e90-111">Open the mailbox in Outlook on the web, and click **Settings** \> **Options** \> **Organize email** \> **Inbox rules**.</span></span>
    
2. <span data-ttu-id="66e90-112">在页面底部, 单击 "**如果规则未正常工作", 请单击此处生成诊断报告**。</span><span class="sxs-lookup"><span data-stu-id="66e90-112">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
    

