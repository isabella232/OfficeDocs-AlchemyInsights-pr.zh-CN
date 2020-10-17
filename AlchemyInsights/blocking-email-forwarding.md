---
title: 726阻止电子邮件转发
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: 610013c4f46e999f1a8715aea14dd557ed8b0e2a
ms.sourcegitcommit: 88f24bb6ced16842de165af416e3f21feae13063
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/15/2020
ms.locfileid: "48478343"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="08a92-102">阻止或取消阻止电子邮件转发</span><span class="sxs-lookup"><span data-stu-id="08a92-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="08a92-103">若要启用或禁用特定邮箱的电子邮件转发，请参阅 [配置电子邮件转发](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)。</span><span class="sxs-lookup"><span data-stu-id="08a92-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="08a92-104">在租户级别，使用出站垃圾邮件策略来控制外部转发。</span><span class="sxs-lookup"><span data-stu-id="08a92-104">On the tenant level, control of external forwarding is done using the outbound spam policy.</span></span> <span data-ttu-id="08a92-105">您可以从 "安全与 [合规中心"](https://protection.office.com/antispam) 中查看出站垃圾邮件筛选器策略，或使用 [HostedOutboundSpamFilterPolicy 命令](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy)。</span><span class="sxs-lookup"><span data-stu-id="08a92-105">You can check the outbound spam filter policy from Security and Compliance Center [here](https://protection.office.com/antispam) or by using the [Get-HostedOutboundSpamFilterPolicy command](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).</span></span>

<span data-ttu-id="08a92-106">如果您遇到以下错误： **"550 5.7.520 访问被拒绝，您的组织不允许外部转发"**，请确保将策略配置为启用外部自动转发。</span><span class="sxs-lookup"><span data-stu-id="08a92-106">If you are getting the following error: **“550 5.7.520 Access denied, Your organization does not allow external forwarding”**, please make sure the policy is configured to enable External Auto-forward.</span></span>

<span data-ttu-id="08a92-107">**注意：** 建议将外部 Autoforward 禁用默认的出站垃圾邮件筛选器策略，并仅为需要外部转发的用户启用这些用户的自定义策略，并对其启用。</span><span class="sxs-lookup"><span data-stu-id="08a92-107">**Note:** It is recommended to keep the External Autoforward disabled on your default outbound spam filter policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="08a92-108">若要了解详细信息，请参阅在 [Office 365 中配置外部电子邮件转发](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)。</span><span class="sxs-lookup"><span data-stu-id="08a92-108">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>