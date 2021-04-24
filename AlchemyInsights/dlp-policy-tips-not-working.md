---
title: DLP 策略提示无法工作
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 8a3b8175c077b77d1c9b5d859012faddcb1fa3a0
ms.sourcegitcommit: 099704f7f4bdf122d09bb4f7cc71d36fc77a7fcf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2021
ms.locfileid: "51958692"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="8836b-102">DLP 策略提示问题</span><span class="sxs-lookup"><span data-stu-id="8836b-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="8836b-103">**重要信息：** 在这段前所未有的时期，我们正在采取措施确保 SharePoint Online 和 OneDrive 服务高度可用，请访问 [SharePoint Online 临时功能调整](https://aka.ms/ODSPAdjustments)，获取详细信息。</span><span class="sxs-lookup"><span data-stu-id="8836b-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="8836b-104">若要在完全强制执行模式下在安全与合规&配置 DLP 策略的策略提示，请执行下列操作：</span><span class="sxs-lookup"><span data-stu-id="8836b-104">To configure policy tips on your DLP policy in the Security & Compliance center in full enforcement mode, do the following:</span></span>

- <span data-ttu-id="8836b-105">确保已在 DLP **规则** 上启用策略提示。</span><span class="sxs-lookup"><span data-stu-id="8836b-105">Ensure policy tips have been **enabled** on the DLP rule.</span></span> <span data-ttu-id="8836b-106">有关步骤，请参阅 [发送电子邮件通知和显示 DLP 策略的策略提示](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)。</span><span class="sxs-lookup"><span data-stu-id="8836b-106">For steps, see [Send email notifications and show policy tips for DLP policies](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="8836b-107">确保内容与触发敏感信息类型实体定义中概述的规则 [所需的内容匹配](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)。</span><span class="sxs-lookup"><span data-stu-id="8836b-107">Ensure your content matches what is required to trigger the rule outlined in [Sensitive information type entity definitions](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="8836b-108">策略提示同时显示在 OWA 和 Outlook 中。</span><span class="sxs-lookup"><span data-stu-id="8836b-108">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="8836b-109">但是，在使用 Outlook 2013 或更高版本时，策略提示仅在某些条件下显示。</span><span class="sxs-lookup"><span data-stu-id="8836b-109">However, when using Outlook 2013 or later, policy tips are displayed only under certain conditions.</span></span> <span data-ttu-id="8836b-110">有关特定条件列表，请参阅 Supported [conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)。</span><span class="sxs-lookup"><span data-stu-id="8836b-110">For the specific conditions list, see [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).</span></span>

<span data-ttu-id="8836b-111">有关 DLP 策略提示的信息，请参阅 [DLP Policy Tips Reference](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps) and Support Matrix for DLP Policy [tips](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps)。</span><span class="sxs-lookup"><span data-stu-id="8836b-111">For information on DLP Policy tips, see [DLP Policy Tips Reference](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps) and [Support Matrix for DLP Policy tips](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps).</span></span>