---
title: 来自电子邮件的事件的疑难解答
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658724"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="41de7-102">来自电子邮件的事件的疑难解答</span><span class="sxs-lookup"><span data-stu-id="41de7-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="41de7-103">验证是否已为邮箱启用该功能：**Get-EventsFromEmailConfiguration -Identity <mailbox>**</span><span class="sxs-lookup"><span data-stu-id="41de7-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="41de7-104">然后查看“来自电子邮件的事件”日志 **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="41de7-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="41de7-105">在“来自电子邮件的事件”日志中，找到与邮箱中的相应项目匹配的 InternetMessageId。</span><span class="sxs-lookup"><span data-stu-id="41de7-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="41de7-106">TrustScore 决定是否添加该项目。</span><span class="sxs-lookup"><span data-stu-id="41de7-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="41de7-107">仅当 TrustScore =“Trusted”时才会添加事件。</span><span class="sxs-lookup"><span data-stu-id="41de7-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="41de7-108">TrustScore 由 SPF、Dkim 或 Dmarc 属性决定，它们位于邮件头中。</span><span class="sxs-lookup"><span data-stu-id="41de7-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="41de7-109">若要查看这些属性，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="41de7-109">To view these properties:</span></span>

<span data-ttu-id="41de7-110">**桌面版 Outlook**</span><span class="sxs-lookup"><span data-stu-id="41de7-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="41de7-111">打开相应项目</span><span class="sxs-lookup"><span data-stu-id="41de7-111">Open the item</span></span>
- <span data-ttu-id="41de7-112">“文件”->“属性”->“Internet 邮件头”</span><span class="sxs-lookup"><span data-stu-id="41de7-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="41de7-113">或</span><span class="sxs-lookup"><span data-stu-id="41de7-113">or</span></span>

<span data-ttu-id="41de7-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="41de7-114">**MFCMapi**</span></span>

- <span data-ttu-id="41de7-115">导航到收件箱中的相应项目</span><span class="sxs-lookup"><span data-stu-id="41de7-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="41de7-116">查找 PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="41de7-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="41de7-117">系统将在传输和路由过程中确定并记录这些属性。</span><span class="sxs-lookup"><span data-stu-id="41de7-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="41de7-118">如需进一步进行故障排除，可能需要跟进有关 SPF、DKIM 和 DMARC 中故障的传输支持。</span><span class="sxs-lookup"><span data-stu-id="41de7-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>