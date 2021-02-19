---
title: 你的用户是否收到恶意电子邮件
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
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 2197e7f195d789193798b80cb092d8046eb6e0be
ms.sourcegitcommit: 3c708a4a349b60b59bc623c44fb78674c685f3c2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/18/2021
ms.locfileid: "50291782"
---
# <a name="did-your-users-receive-malicious-email"></a><span data-ttu-id="6bd91-102">你的用户是否收到恶意电子邮件？</span><span class="sxs-lookup"><span data-stu-id="6bd91-102">Did your users receive malicious email?</span></span>

- <span data-ttu-id="6bd91-103">现在，你可以使用[安全与合规中心中的“管理员提交”](https://sip.protection.office.com/reportsubmission)来 Microsoft 报告恶意电子邮件。</span><span class="sxs-lookup"><span data-stu-id="6bd91-103">You can now report the malicious email to Microsoft using the [Admin Submissions in Security & Compliance Center](https://sip.protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="6bd91-104">提交至 [管理员提交](https://sip.protection.office.com/reportsubmission)中的邮件将会被扫描，以下结果将显示在 **详细信息** 的弹出页面中：</span><span class="sxs-lookup"><span data-stu-id="6bd91-104">Messages that are submitted in [admin submissions](https://sip.protection.office.com/reportsubmission) are scanned, and the following results shown in the **details** flyout:</span></span>

- <span data-ttu-id="6bd91-105">发件人的电子邮件身份验证是否在发送时验证失败。</span><span class="sxs-lookup"><span data-stu-id="6bd91-105">If there was a failure in the sender's email authentication at the time of delivery.</span></span>
- <span data-ttu-id="6bd91-106">任何可能影响或覆盖邮件裁定的策略信息。</span><span class="sxs-lookup"><span data-stu-id="6bd91-106">Information about any policy hits that could have affected or overridden the verdict of a message.</span></span>
- <span data-ttu-id="6bd91-107">当前触发结果，以查看邮件中所包含的 URL 或文件是否是恶意的。</span><span class="sxs-lookup"><span data-stu-id="6bd91-107">Current detonation results to see if the URLs or files contained in the message were malicious or not.</span></span>
- <span data-ttu-id="6bd91-108">评价员的反馈</span><span class="sxs-lookup"><span data-stu-id="6bd91-108">Feedback from graders</span></span>

<span data-ttu-id="6bd91-109">如果找到了覆盖，则应该会在数分钟内完成重新扫描。</span><span class="sxs-lookup"><span data-stu-id="6bd91-109">If an override was found, the rescan should complete in several minutes.</span></span> <span data-ttu-id="6bd91-110">如果电子邮件身份验证中不存在问题，或者覆盖对传递没有影响的话，则评价员的反馈可能需要多达一天的时间。</span><span class="sxs-lookup"><span data-stu-id="6bd91-110">If there wasn't a problem in email authentication or if the delivery wasn't affected by an override, then the feedback from graders could take up to a day.</span></span>

<span data-ttu-id="6bd91-111">如果不同意邮件、URL 或文件的最终裁定（被阻止与未阻止），请在一天之后再次提交该邮件以进行重新扫描。</span><span class="sxs-lookup"><span data-stu-id="6bd91-111">If you disagree with the final verdict on a message, URL or file (blocked vs. not blocked), submit the message again after a day for rescan.</span></span> <span data-ttu-id="6bd91-112">再次提交邮件后，裁定更改的几率是相当高的。</span><span class="sxs-lookup"><span data-stu-id="6bd91-112">The chances are high that the verdict would change after submitting the message again.</span></span>

<span data-ttu-id="6bd91-113">同时，你可按照[本文](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)中的说明从用户的收件箱中删除恶意电子邮件。</span><span class="sxs-lookup"><span data-stu-id="6bd91-113">Meanwhile, you can remove malicious email from user inboxes by following the instructions in [this article](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).</span></span>

- <span data-ttu-id="6bd91-114">使用 Microsoft Defender for Office 365 的客户可以：</span><span class="sxs-lookup"><span data-stu-id="6bd91-114">Customers with Microsoft Defender for Office 365 can:</span></span>
    - <span data-ttu-id="6bd91-115">使用 [威胁资源管理器“查找”和”删除可疑电子邮件”](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)</span><span class="sxs-lookup"><span data-stu-id="6bd91-115">use [Threat Explorer to Find and Delete Suspicious email](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)</span></span>
    - <span data-ttu-id="6bd91-116">[使用安全链接阻止访问](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links)恶意 URL</span><span class="sxs-lookup"><span data-stu-id="6bd91-116">[use Safe Links to block access](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) to a malicious URL</span></span>
    - <span data-ttu-id="6bd91-117">跟踪已单击和已访问恶意 URL 的用户：[查看网络钓鱼 URL 并单击裁定数据](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)</span><span class="sxs-lookup"><span data-stu-id="6bd91-117">track users who clicked and accessed malicious URLs: [View phishing URL and click verdict data](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)</span></span>
    - <span data-ttu-id="6bd91-118">手动[开始“自动调查”](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)</span><span class="sxs-lookup"><span data-stu-id="6bd91-118">manually [start an Automated Investigation](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)</span></span>

<span data-ttu-id="6bd91-119">你也可以按照[防范恶意 URL 和文件](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats)中的说明，保护自己免受恶意文件和 URL 的侵害。</span><span class="sxs-lookup"><span data-stu-id="6bd91-119">You can also protect against malicious files and URLs by following the instructions in [Protection from malicious URLs and files](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).</span></span>