---
title: 隔离邮件会发生什么情况？
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: de7ea8011af792cd01963c44f8a60915747c3c11
ms.sourcegitcommit: 1f998ca586c90330fde515525432072f766d485b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2021
ms.locfileid: "50520537"
---
# <a name="what-happens-to-quarantined-messages"></a><span data-ttu-id="3c0df-102">隔离邮件会发生什么情况？</span><span class="sxs-lookup"><span data-stu-id="3c0df-102">What happens to quarantined messages?</span></span>

<span data-ttu-id="3c0df-103">如果选择不执行任何操作，邮件到期后，将由 Office 365 自动删除。</span><span class="sxs-lookup"><span data-stu-id="3c0df-103">If you choose to do nothing, the message will be deleted by Office 365 automatically upon expiration.</span></span> <span data-ttu-id="3c0df-104">请注意以下事项：</span><span class="sxs-lookup"><span data-stu-id="3c0df-104">Note the following:</span></span>

1. <span data-ttu-id="3c0df-105">默认情况下，垃圾邮件、批量邮件、恶意软件和网络钓鱼邮件在隔离中保留 15 天。</span><span class="sxs-lookup"><span data-stu-id="3c0df-105">By default, spam, bulk, malware, and phishing messages are kept in quarantine for 15 days.</span></span>
2. <span data-ttu-id="3c0df-106">与邮件流规则匹配的隔离邮件在隔离中保留 7 (无法自定义此) 。</span><span class="sxs-lookup"><span data-stu-id="3c0df-106">A quarantined message that matches a mail flow rule is kept in quarantine for 7 days (you can't customize this).</span></span>
3. <span data-ttu-id="3c0df-107">Office 365 从隔离区删除邮件后，你无法将其恢复。</span><span class="sxs-lookup"><span data-stu-id="3c0df-107">When Office 365 deletes a message from quarantine, you can't get it back.</span></span>
4. <span data-ttu-id="3c0df-108">如果愿意，可以在内容筛选器策略中通过使用"将垃圾邮件保留 () 天数"来更改隔离邮件的保留期。</span><span class="sxs-lookup"><span data-stu-id="3c0df-108">If you like, you can change the retention period for quarantined messages by using the Retain spam for (days) setting in your content filter policies.</span></span>
