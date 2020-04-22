---
title: 敏感度标签未显示
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 72dc88a55b55954f34c95fa5b5038f472261c5bb
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758365"
---
# <a name="sensitivity-labels-not-appearing"></a><span data-ttu-id="126a5-102">敏感度标签未显示</span><span class="sxs-lookup"><span data-stu-id="126a5-102">Sensitivity labels not appearing</span></span>

<span data-ttu-id="126a5-103">敏感度标签允许您对敏感内容进行分类和帮助保护。</span><span class="sxs-lookup"><span data-stu-id="126a5-103">Sensitivity labels allow you to classify and help protect your sensitive content.</span></span> <span data-ttu-id="126a5-104">它们可以在 Microsoft 365 合规性中心、Microsoft 365 安全中心或 Microsoft 365 安全 & 合规性中心下的 "分类 > 敏感度标签" 下创建。</span><span class="sxs-lookup"><span data-stu-id="126a5-104">They can be created in the Microsoft 365 compliance center, Microsoft 365 security center, or Microsoft 365 security & Compliance Center under Classification > Sensitivity labels.</span></span> <span data-ttu-id="126a5-105">若要了解有关此功能的详细信息，请参阅[敏感度标签概述](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels)。</span><span class="sxs-lookup"><span data-stu-id="126a5-105">To learn more about this feature, see [Overview of sensitivity labels](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels).</span></span>

<span data-ttu-id="126a5-106">如果您配置了灵敏度标签但它们未显示在 Office 应用中，请检查以下各项：</span><span class="sxs-lookup"><span data-stu-id="126a5-106">If you configured your sensitivity labels but they aren't appearing in the Office apps, check the following:</span></span>

- <span data-ttu-id="126a5-107">确认是否已将敏感度标签[发布](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do)到所需的用户和组。</span><span class="sxs-lookup"><span data-stu-id="126a5-107">Confirm that the sensitivity label has been [published](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do) to the users and groups that you want.</span></span>

- <span data-ttu-id="126a5-108">确认用户正在使用支持敏感度标签的应用程序-请参阅[文档中的敏感度标签](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable)。</span><span class="sxs-lookup"><span data-stu-id="126a5-108">Confirm that the user is using an app that supports sensitivity labels - see [sensitivity labels in your document](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).</span></span>

- <span data-ttu-id="126a5-109">如果要[迁移 Azure 信息保护标签](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)，请注意[此处](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)列出的注意事项。</span><span class="sxs-lookup"><span data-stu-id="126a5-109">If you're [migrating Azure Information Protection labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), be aware of the considerations listed [here](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span></span>

- <span data-ttu-id="126a5-110">数据丢失防护（DLP）支持：目前，在 DLP 策略中，仅保留标签可用作条件。</span><span class="sxs-lookup"><span data-stu-id="126a5-110">Data loss prevention (DLP) support: Currently, only retention labels can be used as a condition in DLP policies.</span></span>  <span data-ttu-id="126a5-111">DLP 策略中的敏感度标签支持尚不可用，但我们正在对其进行处理。</span><span class="sxs-lookup"><span data-stu-id="126a5-111">Support for sensitivity labels in a DLP policy is not available yet but we're working on it.</span></span>

- <span data-ttu-id="126a5-112">对敏感度标签启用加密时，您可以选择执行以下操作之一：</span><span class="sxs-lookup"><span data-stu-id="126a5-112">When encryption is enabled on a sensitivity label, you can choose either to:</span></span>
    - <span data-ttu-id="126a5-113">立即分配权限</span><span class="sxs-lookup"><span data-stu-id="126a5-113">Assign permissions now</span></span>
    - <span data-ttu-id="126a5-114">允许用户分配权限</span><span class="sxs-lookup"><span data-stu-id="126a5-114">Let users assign permissions</span></span>


<span data-ttu-id="126a5-115">有关可能存在的问题的详细信息，请参阅[灵敏度标签的已知问题](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc)。</span><span class="sxs-lookup"><span data-stu-id="126a5-115">For more information on possible issues, see [Known issues with sensitivity labels](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span></span>