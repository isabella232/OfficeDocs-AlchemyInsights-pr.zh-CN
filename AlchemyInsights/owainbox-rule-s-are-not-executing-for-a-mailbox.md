---
title: 1332 OWA-收件箱规则未对邮箱执行
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 218a05a8d321b76dd07345ea48d6b3e158cc120e
ms.sourcegitcommit: 77f704672b7c7de541899e25c022ff10c111e304
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2019
ms.locfileid: "36204050"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="c47ce-102">收件箱规则不能按预期工作</span><span class="sxs-lookup"><span data-stu-id="c47ce-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="c47ce-103">验证以下设置:</span><span class="sxs-lookup"><span data-stu-id="c47ce-103">Verify the following settings:</span></span>

- <span data-ttu-id="c47ce-104">可以基于收件箱规则自动重定向、转发或答复邮件一次。</span><span class="sxs-lookup"><span data-stu-id="c47ce-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="c47ce-105">重定向规则 (收件箱规则或邮件流规则, 也称为传输规则) 最多可以向邮件中添加10个转发收件人。</span><span class="sxs-lookup"><span data-stu-id="c47ce-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="c47ce-106">有关详细信息, 请参阅[日记、Transport 和收件箱规则限制](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)。</span><span class="sxs-lookup"><span data-stu-id="c47ce-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="c47ce-107">收件箱规则在备用日记邮箱中不起作用。</span><span class="sxs-lookup"><span data-stu-id="c47ce-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="c47ce-108">有关备用日记邮箱的详细信息, 请参阅[备用日记邮箱](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)。</span><span class="sxs-lookup"><span data-stu-id="c47ce-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="c47ce-109">若要解决这些问题, 请参阅[KB 2829319](https://support.microsoft.com/kb/2829319)。</span><span class="sxs-lookup"><span data-stu-id="c47ce-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="c47ce-110">如果未应用以前的问题, 请在将问题升级到 Microsoft 支持之前运行 "收件箱规则诊断报告":</span><span class="sxs-lookup"><span data-stu-id="c47ce-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="c47ce-111">打开 web 上的 Outlook 中的邮箱, 然后单击</span><span class="sxs-lookup"><span data-stu-id="c47ce-111">Open the mailbox in Outlook on the web, and click</span></span> <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 <span data-ttu-id="c47ce-112">**"设置** > **" 查看所有 Outlook 设置** > **邮件** > **规则**。</span><span class="sxs-lookup"><span data-stu-id="c47ce-112">**Settings** > **View all Outlook Settings** > **Mail** > **Rules**.</span></span>

2. <span data-ttu-id="c47ce-113">在页面底部, 单击 "**如果规则未正常工作", 请单击此处生成诊断报告**。</span><span class="sxs-lookup"><span data-stu-id="c47ce-113">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
