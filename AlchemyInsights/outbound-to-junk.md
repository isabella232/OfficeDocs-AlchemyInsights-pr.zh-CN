---
title: 出站电子邮件至垃圾邮件文件夹
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 869cd3d9fb8e5fce291244e4a39754d074b11358
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511714"
---
# <a name="outbound-email-to-junk-email-folder"></a><span data-ttu-id="91ab7-102">出站电子邮件至垃圾邮件文件夹</span><span class="sxs-lookup"><span data-stu-id="91ab7-102">Outbound email to Junk Email folder</span></span>

<span data-ttu-id="91ab7-103">如果要查看标记为垃圾邮件的出站邮件，请执行以下步骤：</span><span class="sxs-lookup"><span data-stu-id="91ab7-103">If you're seeing outbound messages being marked as Junk, do the following steps:</span></span>

- <span data-ttu-id="91ab7-104">如果还未配置，请考虑[配置出站垃圾邮件策略通知](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy)。</span><span class="sxs-lookup"><span data-stu-id="91ab7-104">If you haven't already, consider [configuring outbound spam policy notifications](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).</span></span>

- <span data-ttu-id="91ab7-105">使用[邮件跟踪](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc)查看出站邮件是否具有其他详细信息的事件值**垃圾邮件**：**使用高风险传递池**。</span><span class="sxs-lookup"><span data-stu-id="91ab7-105">Use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) to see if the outbound message has the event value **Spam** with the additional detail: **Use high risk delivery pool**.</span></span>

  <span data-ttu-id="91ab7-106">对于这些邮件，请检查邮件内容以查看可能被视为垃圾邮件的内容。</span><span class="sxs-lookup"><span data-stu-id="91ab7-106">For these messages, check the message content to see what might be considered spam.</span></span> <span data-ttu-id="91ab7-107">例如，签名有时可能会导致许多用户出现问题。</span><span class="sxs-lookup"><span data-stu-id="91ab7-107">For example, signatures can sometimes cause problems for many users.</span></span>

  <span data-ttu-id="91ab7-108">如果您有多个将被标记为垃圾邮件的合法出站邮件的示例，请打开支持票证，并请求支持代理将您的邮件作为误报提交给垃圾邮件分析员。</span><span class="sxs-lookup"><span data-stu-id="91ab7-108">If you have multiple examples of legitimate outbound messages that are being marked as Junk, open a support ticket and ask the support agent to submit your messages as false positives to our spam analysts.</span></span> <span data-ttu-id="91ab7-109">准备提供包含所有邮件头的示例邮件。</span><span class="sxs-lookup"><span data-stu-id="91ab7-109">Be prepared to provide sample messages that include all message headers.</span></span>
