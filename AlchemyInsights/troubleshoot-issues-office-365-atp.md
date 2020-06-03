---
title: 解决 Office 365 高级威胁防护（ATP）的问题
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: f1dc675c8a8217ea2824ad46e029bfa303303e6a
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511102"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="099ce-102">解决 Office 365 ATP 中的问题</span><span class="sxs-lookup"><span data-stu-id="099ce-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="099ce-103">**注意电子邮件传递是否延迟**？</span><span class="sxs-lookup"><span data-stu-id="099ce-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="099ce-104">尝试对 ATP 安全附件策略使用动态传递选项。</span><span class="sxs-lookup"><span data-stu-id="099ce-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="099ce-105">这将避免电子邮件传递延迟，同时防止收件人受到恶意文件的攻击。</span><span class="sxs-lookup"><span data-stu-id="099ce-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="099ce-106">**是否要报告误报或漏报**？</span><span class="sxs-lookup"><span data-stu-id="099ce-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="099ce-107">使用此链接提交您的文件以供分析：[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="099ce-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="099ce-108">**您是否知道您可以为组织中的人员发送的电子邮件启用 ATP 安全链接保护**？</span><span class="sxs-lookup"><span data-stu-id="099ce-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="099ce-109">请按以下步骤操作：</span><span class="sxs-lookup"><span data-stu-id="099ce-109">Follow these steps:</span></span>
    1. <span data-ttu-id="099ce-110">转到 https://protection.office.com ，然后登录。</span><span class="sxs-lookup"><span data-stu-id="099ce-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="099ce-111">转到 "**威胁管理**  >  **策略**  >  **安全链接**"。</span><span class="sxs-lookup"><span data-stu-id="099ce-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="099ce-112">在 "**适用于特定收件人的策略**" 下，编辑（或添加）策略。</span><span class="sxs-lookup"><span data-stu-id="099ce-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="099ce-113">选择 "**将安全链接应用于在组织内发送的邮件"**。</span><span class="sxs-lookup"><span data-stu-id="099ce-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="099ce-114">保存您的策略，并大约等待30分钟，以使更改在您的数据中心中工作。</span><span class="sxs-lookup"><span data-stu-id="099ce-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="099ce-115">若要获取有关 ATP 的更多帮助，请参阅[Office 365 高级威胁防护](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp)。</span><span class="sxs-lookup"><span data-stu-id="099ce-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>