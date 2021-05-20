---
title: Microsoft Defender for Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 91d73853d3ea67d6c6954fffb32dd1428e3d9976
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545258"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a><span data-ttu-id="e219a-102">Microsoft Defender for Office 365</span><span class="sxs-lookup"><span data-stu-id="e219a-102">Troubleshooting Microsoft Defender for Office 365</span></span>

- <span data-ttu-id="e219a-103">**你是否注意到邮件传递延迟？**</span><span class="sxs-lookup"><span data-stu-id="e219a-103">**Do you notice delays in message delivery?**</span></span> <span data-ttu-id="e219a-104">使用[Microsoft](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) Defender for Office 365 保险箱 策略中的"动态传递"选项。</span><span class="sxs-lookup"><span data-stu-id="e219a-104">Use the [Dynamic Delivery](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your Microsoft Defender for Office 365 Safe Attachments policy.</span></span> <span data-ttu-id="e219a-105">这有助于避免邮件延迟，同时保护收件人免受恶意文件的攻击。</span><span class="sxs-lookup"><span data-stu-id="e219a-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="e219a-106">**是否要向 Microsoft 报告误报或漏报？**</span><span class="sxs-lookup"><span data-stu-id="e219a-106">**Do you want to report false positives or false negatives to Microsoft?**</span></span> <span data-ttu-id="e219a-107">使用 [提交资源管理器](https://protection.office.com/reportsubmission)。</span><span class="sxs-lookup"><span data-stu-id="e219a-107">Use [Submissions Explorer](https://protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="e219a-108">-\*\* 您是否知道您可以为在保险箱收件人之间发送的内部电子邮件启用链接保护？\*\* 请按照以下步骤操作：</span><span class="sxs-lookup"><span data-stu-id="e219a-108">-\*\* Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?\*\* Follow these steps:</span></span>

  1. <span data-ttu-id="e219a-109">转到 ， [https://protection.office.com](https://protection.office.com) 然后使用全局管理员或安全管理员帐户登录。</span><span class="sxs-lookup"><span data-stu-id="e219a-109">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="e219a-110">在左侧导航窗格中 **的"威胁** 管理"下 **，选择"** 策略 \> **保险箱链接"。**</span><span class="sxs-lookup"><span data-stu-id="e219a-110">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="e219a-111">在"**应用于整个组织的策略"部分**，选择策略并单击"编辑 **"。**</span><span class="sxs-lookup"><span data-stu-id="e219a-111">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="e219a-112">在 **设置"** 下，**启用"将安全链接应用于在组织内部发送的邮件"。**</span><span class="sxs-lookup"><span data-stu-id="e219a-112">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
