---
title: Web 上的 Outlook 中的 S/MIME
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 33e94eac6a2982b8036e13d17bf60015f244f2cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053215"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="ed8ed-102">在 Outlook 中加密电子邮件</span><span class="sxs-lookup"><span data-stu-id="ed8ed-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="ed8ed-103">Office 365 邮件加密是基于 Microsoft Azure 权限管理（Azure RMS）构建的，这是 Azure 信息保护的一部分。</span><span class="sxs-lookup"><span data-stu-id="ed8ed-103">Office 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="ed8ed-104">如果你的订阅包括 Azure 权限管理或 Azure 信息保护，**则无需执行任何操作来手动启用或激活**权限管理服务。</span><span class="sxs-lookup"><span data-stu-id="ed8ed-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="ed8ed-105">根据客户反馈，我们将不再启用 Exchange 邮件流规则，以在默认情况下，在租户中自动对包含特定类型敏感信息的出站电子邮件进行加密。</span><span class="sxs-lookup"><span data-stu-id="ed8ed-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="ed8ed-106">相反，我们将提供有关如何进行此操作的详细说明。</span><span class="sxs-lookup"><span data-stu-id="ed8ed-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="ed8ed-107">有关如何创建传输规则以加密敏感信息的其他详细信息，请参阅[本文](https://aka.ms/OmeEtr)。</span><span class="sxs-lookup"><span data-stu-id="ed8ed-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="ed8ed-108">如果使用 Web 上的 Outlook （以前称为**OWA**）：撰写电子邮件时，只需在 OWA 中单击 "**保护**" 即可。</span><span class="sxs-lookup"><span data-stu-id="ed8ed-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="ed8ed-109">这将应用 "不转发" 权限。</span><span class="sxs-lookup"><span data-stu-id="ed8ed-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="ed8ed-110">单击 "**更改权限**"，然后选择 "**加密**" 仅加密邮件。</span><span class="sxs-lookup"><span data-stu-id="ed8ed-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="ed8ed-111">如果使用**outlook 客户端**：从 outlook 2013 或2016发送加密邮件，或 outlook 2016 for Mac，请选择 "**选项** > **权限**"，然后选择所需的保护选项。</span><span class="sxs-lookup"><span data-stu-id="ed8ed-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="ed8ed-112">若要自动对发送给特定收件人或外部合作伙伴组织的**所有电子邮件进行加密**，需要在 Exchange 管理中心中创建邮件流传输规则。</span><span class="sxs-lookup"><span data-stu-id="ed8ed-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="ed8ed-113">[本支持文章](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities)中提供了详细说明。</span><span class="sxs-lookup"><span data-stu-id="ed8ed-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

