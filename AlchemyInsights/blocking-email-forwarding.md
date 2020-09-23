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
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219845"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="f275b-102">阻止或取消阻止电子邮件转发</span><span class="sxs-lookup"><span data-stu-id="f275b-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="f275b-103">若要启用或禁用特定邮箱的电子邮件转发，请参阅 [配置电子邮件转发](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)。</span><span class="sxs-lookup"><span data-stu-id="f275b-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="f275b-104">在租户级别上，外部转发的控制使用出站反垃圾邮件策略完成。</span><span class="sxs-lookup"><span data-stu-id="f275b-104">On the tenant level, control of External forwarding is done using the outbound anti-spam policy.</span></span> <span data-ttu-id="f275b-105">如果将其设置为 Off 或 Automatic，它可能会阻止使用 "550 5.7.520 访问" 拒绝的电子邮件转发，而您的组织不允许外部转发 "错误。</span><span class="sxs-lookup"><span data-stu-id="f275b-105">If it is set to Off or Automatic, it might block email forwarding with the “550 5.7.520 Access denied, Your organization does not allow external forwarding” error.</span></span> <span data-ttu-id="f275b-106">随后，如果将转发设置为 "已阻止"，则表明您的用户将看到的错误。</span><span class="sxs-lookup"><span data-stu-id="f275b-106">Subsequently, if forwarding was set to be blocked, that is the error your users will see.</span></span>

<span data-ttu-id="f275b-107">如果正在阻止转发，请确保将策略配置为启用外部 Autoforward。</span><span class="sxs-lookup"><span data-stu-id="f275b-107">If forwarding is being blocked, please make sure the policy is configured to enable External Autoforward.</span></span> <span data-ttu-id="f275b-108">您可以从 "安全和合规中心" 中检查出站垃圾邮件筛选器策略，也可以通过运行命令 HostedOutboundSpamFilterPolicy |fl 名称，AutoForwardingMode。</span><span class="sxs-lookup"><span data-stu-id="f275b-108">You can check the Outbound Spam Filter Policy from Security and Compliance Center or by running command Get-HostedOutboundSpamFilterPolicy | fl name,AutoForwardingMode.</span></span> <span data-ttu-id="f275b-109">如果要设置 Autoforward 阻止，相同的命令将立即告知您的策略状态。</span><span class="sxs-lookup"><span data-stu-id="f275b-109">If you want to set up Autoforward blocking, the same command will tell you the state of policy now.</span></span>

<span data-ttu-id="f275b-110">注意：建议将外部 Autoforward 禁用在默认出站垃圾邮件筛选器策略上，并仅为需要外部转发的用户启用这些用户的自定义策略，并启用此策略。</span><span class="sxs-lookup"><span data-stu-id="f275b-110">Note: It is recommended to keep the External Autoforward disabled on your Default Outbound Spam Filter Policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="f275b-111">若要了解详细信息，请参阅在 [Office 365 中配置外部电子邮件转发](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)。</span><span class="sxs-lookup"><span data-stu-id="f275b-111">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>