---
title: Microsoft Defender for Endpoints 的计算机载入问题
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 7ccec69f8ab43f277978176519a7f8f8df443846
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/19/2021
ms.locfileid: "50901557"
---
# <a name="issues-with-onboarding-machines-to-microsoft-defender-for-endpoints"></a><span data-ttu-id="80484-102">Microsoft Defender for Endpoints 的计算机载入问题</span><span class="sxs-lookup"><span data-stu-id="80484-102">Issues with onboarding machines to Microsoft Defender for Endpoints</span></span>

<span data-ttu-id="80484-103">将计算机载入到 MDE 服务时可能会遇到问题。</span><span class="sxs-lookup"><span data-stu-id="80484-103">You might have issues with onboarding machines to MDE service.</span></span> <span data-ttu-id="80484-104">如果可以访问最终用户计算机，请按照下列步骤进行操作：</span><span class="sxs-lookup"><span data-stu-id="80484-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="80484-105">下载 [MDE Client Analyzer](https://aka.ms/betamdeanalyzer) 诊断工具的最新预览版本。</span><span class="sxs-lookup"><span data-stu-id="80484-105">Download the latest preview version of the [MDE Client Analyzer](https://aka.ms/betamdeanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="80484-106">右键单击 **MDEClientAnalyzer.cmd** 并选择“以管理员角色运行”。</span><span class="sxs-lookup"><span data-stu-id="80484-106">Right click **MDEClientAnalyzer.cmd** and select ‘Run as administrator’.</span></span>
3. <span data-ttu-id="80484-107">按照 **MDEClientAnalyzer.htm** 中的任何指导建议操作。</span><span class="sxs-lookup"><span data-stu-id="80484-107">Follow any guidance suggested in **MDEClientAnalyzer.htm**.</span></span>
4. <span data-ttu-id="80484-108">有关详细日志，请查看创建的名为 **MDEClientAnalyzerResult** 的子文件夹。</span><span class="sxs-lookup"><span data-stu-id="80484-108">For more verbose logs, review the created sub-folder named **MDEClientAnalyzerResult**.</span></span>
5. <span data-ttu-id="80484-109">如果需要其他指导，请与 [Microsoft Defender for Endpoint 支持](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support)联系，并提供生成的 MDEClientAnalyzerResult.zip 文件以供分析。</span><span class="sxs-lookup"><span data-stu-id="80484-109">If additional guidance is needed, contact [Microsoft Defender for Endpoint support](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) and provide the resulting MDEClientAnalyzerResult.zip file for analysis.</span></span>
