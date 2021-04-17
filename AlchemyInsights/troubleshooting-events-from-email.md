---
title: 来自电子邮件的事件的疑难解答
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834829"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="4b2cb-102">来自电子邮件的事件的疑难解答</span><span class="sxs-lookup"><span data-stu-id="4b2cb-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="4b2cb-103">验证是否已为邮箱启用该功能：**Get-EventsFromEmailConfiguration -Identity <mailbox>**</span><span class="sxs-lookup"><span data-stu-id="4b2cb-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="4b2cb-104">然后查看“来自电子邮件的事件”日志 **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="4b2cb-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="4b2cb-105">在“来自电子邮件的事件”日志中，找到与邮箱中的相应项目匹配的 InternetMessageId。</span><span class="sxs-lookup"><span data-stu-id="4b2cb-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="4b2cb-106">TrustScore 决定是否添加该项目。</span><span class="sxs-lookup"><span data-stu-id="4b2cb-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="4b2cb-107">仅当 TrustScore =“Trusted”时才会添加事件。</span><span class="sxs-lookup"><span data-stu-id="4b2cb-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="4b2cb-108">TrustScore 由 SPF、Dkim 或 Dmarc 属性决定，它们位于邮件头中。</span><span class="sxs-lookup"><span data-stu-id="4b2cb-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="4b2cb-109">若要查看这些属性，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="4b2cb-109">To view these properties:</span></span>

<span data-ttu-id="4b2cb-110">**桌面版 Outlook**</span><span class="sxs-lookup"><span data-stu-id="4b2cb-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="4b2cb-111">打开相应项目</span><span class="sxs-lookup"><span data-stu-id="4b2cb-111">Open the item</span></span>
- <span data-ttu-id="4b2cb-112">“文件”->“属性”->“Internet 邮件头”</span><span class="sxs-lookup"><span data-stu-id="4b2cb-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="4b2cb-113">或</span><span class="sxs-lookup"><span data-stu-id="4b2cb-113">or</span></span>

<span data-ttu-id="4b2cb-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="4b2cb-114">**MFCMapi**</span></span>

- <span data-ttu-id="4b2cb-115">导航到收件箱中的相应项目</span><span class="sxs-lookup"><span data-stu-id="4b2cb-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="4b2cb-116">查找 PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="4b2cb-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="4b2cb-117">系统将在传输和路由过程中确定并记录这些属性。</span><span class="sxs-lookup"><span data-stu-id="4b2cb-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="4b2cb-118">如需进一步进行故障排除，可能需要跟进有关 SPF、DKIM 和 DMARC 中故障的传输支持。</span><span class="sxs-lookup"><span data-stu-id="4b2cb-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>