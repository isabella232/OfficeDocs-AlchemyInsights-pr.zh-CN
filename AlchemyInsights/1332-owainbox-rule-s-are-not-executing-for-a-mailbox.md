---
title: 1332 OWA-收件箱规则不执行的邮箱
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: f090d0a9d84bc6a4d1a1f4c0af55102d4b0ddfbe
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29459863"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="1f048-102">收件箱规则没有按预期工作</span><span class="sxs-lookup"><span data-stu-id="1f048-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="1f048-103">验证以下设置：</span><span class="sxs-lookup"><span data-stu-id="1f048-103">Verify the following settings:</span></span>
  
- <span data-ttu-id="1f048-p101">可以重定向一条消息，转发或答复以自动基于收件箱规则仅一次。（收件箱规则或邮件流规则，也称为传输规则） 的重定向规则可以将最多个十个转接收件人添加到一条消息。有关详细信息，请参阅[日记、 传输和收件箱规则限制](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)。</span><span class="sxs-lookup"><span data-stu-id="1f048-p101">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time. A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message. For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>
    
- <span data-ttu-id="1f048-p102">收件箱规则对备用日记邮箱不起作用。有关备用日记邮箱的详细信息，请参阅[备用日记邮箱](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)。</span><span class="sxs-lookup"><span data-stu-id="1f048-p102">Inbox rules don't work on the alternate journaling mailbox. For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>
    
<span data-ttu-id="1f048-109">若要解决这些问题，请参阅[KB 2829319](https://support.microsoft.com/kb/2829319)。</span><span class="sxs-lookup"><span data-stu-id="1f048-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>
  
<span data-ttu-id="1f048-110">如果没有应用上述问题，先升级到 Microsoft 支持问题运行的收件箱规则诊断报告：</span><span class="sxs-lookup"><span data-stu-id="1f048-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>
  
1. <span data-ttu-id="1f048-111">在 web 上的 Outlook 中打开邮箱并单击**设置** \> **选项** \> **组织电子邮件** \> **收件箱规则**。</span><span class="sxs-lookup"><span data-stu-id="1f048-111">Open the mailbox in Outlook on the web, and click **Settings** \> **Options** \> **Organize email** \> **Inbox rules**.</span></span>
    
2. <span data-ttu-id="1f048-112">在页面的底部，单击**如果规则未正常运行单击此处以生成诊断报告**。</span><span class="sxs-lookup"><span data-stu-id="1f048-112">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
    

