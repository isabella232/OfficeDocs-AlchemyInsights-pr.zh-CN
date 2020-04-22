---
title: 反垃圾邮件-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 307b738c40c620d057e68eff7d218c8c9b5eb665
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676487"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="f38ca-102">修复错误代码5.7.23 的电子邮件传递问题</span><span class="sxs-lookup"><span data-stu-id="f38ca-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="f38ca-103">在 web 上的公开发布的 SPF 或 DNS 记录检查器中验证您的域的 SPF DNS 记录。</span><span class="sxs-lookup"><span data-stu-id="f38ca-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="f38ca-104">确认出站邮件未被 Microsoft 标识为 "垃圾邮件"，并通过[高风险传递池](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages)进行路由。</span><span class="sxs-lookup"><span data-stu-id="f38ca-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="f38ca-105">高风险传递池中的邮件不会通过 SPF 检查，因此目标电子邮件组织不接受这些邮件。</span><span class="sxs-lookup"><span data-stu-id="f38ca-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="f38ca-106">如果问题仍然存在，则可能需要联系您尝试向其发送电子邮件的邮件主机的管理员。</span><span class="sxs-lookup"><span data-stu-id="f38ca-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="f38ca-107">记下弹跳消息中提供的详细外部错误。</span><span class="sxs-lookup"><span data-stu-id="f38ca-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="f38ca-108">Microsoft 支持可能无法进一步协助。</span><span class="sxs-lookup"><span data-stu-id="f38ca-108">Microsoft support may not be able to assist further.</span></span>
