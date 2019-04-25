---
title: 解决 Office 365 高级威胁防护 (ATP) 的问题
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: dbdfe2ddcc4afd4477f66ffd060ddb7093af8fd6
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2019
ms.locfileid: "32420284"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="d8536-102">解决 Office 365 ATP 中的问题</span><span class="sxs-lookup"><span data-stu-id="d8536-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="d8536-103">**注意电子邮件传递是否延迟**？</span><span class="sxs-lookup"><span data-stu-id="d8536-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="d8536-104">尝试对 ATP 安全附件策略使用动态传递选项。</span><span class="sxs-lookup"><span data-stu-id="d8536-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="d8536-105">这将避免电子邮件传递延迟, 同时防止收件人受到恶意文件的攻击。</span><span class="sxs-lookup"><span data-stu-id="d8536-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="d8536-106">**是否要报告误报或漏报**？</span><span class="sxs-lookup"><span data-stu-id="d8536-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="d8536-107">使用此链接提交您的文件以供分析:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="d8536-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="d8536-108">**您是否知道您可以为组织中的人员发送的电子邮件启用 ATP 安全链接保护**？</span><span class="sxs-lookup"><span data-stu-id="d8536-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="d8536-109">请按以下步骤操作：</span><span class="sxs-lookup"><span data-stu-id="d8536-109">Follow these steps:</span></span>
    1. <span data-ttu-id="d8536-110">转到https://protection.office.com, 然后登录。</span><span class="sxs-lookup"><span data-stu-id="d8536-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="d8536-111">转到 "**威胁管理** > **策略** > **安全链接**"。</span><span class="sxs-lookup"><span data-stu-id="d8536-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="d8536-112">在 "**适用于特定收件人的策略**" 下, 编辑 (或添加) 策略。</span><span class="sxs-lookup"><span data-stu-id="d8536-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="d8536-113">选择 "**将安全链接应用于在组织内发送的邮件"**。</span><span class="sxs-lookup"><span data-stu-id="d8536-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="d8536-114">保存您的策略, 并大约等待30分钟, 以使更改在您的数据中心中工作。</span><span class="sxs-lookup"><span data-stu-id="d8536-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="d8536-115">若要获取有关 ATP 的更多帮助, 请参阅[Office 365 高级威胁防护](https://docs.microsoft.com/office365/securitycompliance/office-365-atp)。</span><span class="sxs-lookup"><span data-stu-id="d8536-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/office365/securitycompliance/office-365-atp).</span></span>