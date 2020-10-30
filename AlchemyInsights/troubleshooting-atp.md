---
title: Microsoft Defender for Office 365 的故障排除
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
ms.openlocfilehash: 2c9543660056ebc02b0bd297f619f20fa6820093
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801433"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a><span data-ttu-id="cb30d-102">Microsoft Defender for Office 365 的故障排除</span><span class="sxs-lookup"><span data-stu-id="cb30d-102">Troubleshooting Microsoft Defender for Office 365</span></span>

- <span data-ttu-id="cb30d-103">您是否注意到邮件传递延迟？</span><span class="sxs-lookup"><span data-stu-id="cb30d-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="cb30d-104">在 ATP 安全附件策略中使用 [动态传递](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) 选项。</span><span class="sxs-lookup"><span data-stu-id="cb30d-104">Use the [Dynamic Delivery](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="cb30d-105">这将有助于避免邮件延迟，同时防止收件人受到恶意文件的攻击。</span><span class="sxs-lookup"><span data-stu-id="cb30d-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="cb30d-106">是否要向 Microsoft 报告误报或漏报？</span><span class="sxs-lookup"><span data-stu-id="cb30d-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="cb30d-107">使用此 [链接](https://www.microsoft.com/wdsi/filesubmission/) 提交文件以进行分析。</span><span class="sxs-lookup"><span data-stu-id="cb30d-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="cb30d-108">您是否知道您可以为组织内的收件人之间发送的内部电子邮件启用安全链接保护？</span><span class="sxs-lookup"><span data-stu-id="cb30d-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="cb30d-109">请按以下步骤操作：</span><span class="sxs-lookup"><span data-stu-id="cb30d-109">Follow these steps:</span></span>

  1. <span data-ttu-id="cb30d-110">转到 [https://protection.office.com](https://protection.office.com) 并使用全局管理员帐户或安全管理员帐户登录。</span><span class="sxs-lookup"><span data-stu-id="cb30d-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="cb30d-111">在 " **威胁管理** " 下方的左侧导航窗格中，选择 " **策略** \> **安全链接** "。</span><span class="sxs-lookup"><span data-stu-id="cb30d-111">In the left navigation pane under **Threat management** , choose **Policy** \> **Safe Links** .</span></span>

  3. <span data-ttu-id="cb30d-112">在 " **适用于整个组织的策略** " 部分中，选择该策略，然后单击 " **编辑** "。</span><span class="sxs-lookup"><span data-stu-id="cb30d-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit** .</span></span>

  4. <span data-ttu-id="cb30d-113">在 " **设置** " 下，启用 " **对组织中发送的邮件应用安全链接** "。</span><span class="sxs-lookup"><span data-stu-id="cb30d-113">Under **Settings** , enable **Apply safe links to messages sent within the organization** .</span></span>
