---
title: 使用 Azure 权限管理的使用情况日志记录
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5506"
- "9002281"
ms.openlocfilehash: 606fcdc5394edab26c60925af28cf2d938aac172
ms.sourcegitcommit: 1dada930649a2625eb6d15910b2bfd5e1e00e5b6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/03/2020
ms.locfileid: "46543743"
---
# <a name="use-usage-logging-for-azure-rights-management"></a><span data-ttu-id="7f544-102">使用 Azure 权限管理的使用情况日志记录</span><span class="sxs-lookup"><span data-stu-id="7f544-102">Use usage logging for Azure Rights Management</span></span>

<span data-ttu-id="7f544-103">默认情况下，所有客户都已启用保护使用情况记录。</span><span class="sxs-lookup"><span data-stu-id="7f544-103">By default, protection usage logging is enabled for all customers.</span></span> <span data-ttu-id="7f544-104">日志被写为租户 Azure 存储中的一系列 blob。</span><span class="sxs-lookup"><span data-stu-id="7f544-104">Logs are written as a series of blobs in Azure storage for your tenant.</span></span> <span data-ttu-id="7f544-105">执行保护操作后，大多数的日志可能需要长达 15 分钟的时间才会出现。</span><span class="sxs-lookup"><span data-stu-id="7f544-105">After a protection action, it might take up to 15 minutes for most logs to appear.</span></span>

<span data-ttu-id="7f544-106">你可以使用保护使用日志执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="7f544-106">You can use protection usage logs to:</span></span>

- <span data-ttu-id="7f544-107">分析商业见解</span><span class="sxs-lookup"><span data-stu-id="7f544-107">Analyze business insights</span></span>

- <span data-ttu-id="7f544-108">监视滥用情况</span><span class="sxs-lookup"><span data-stu-id="7f544-108">Monitor for abuse</span></span>

- <span data-ttu-id="7f544-109">执行鉴定分析</span><span class="sxs-lookup"><span data-stu-id="7f544-109">Perform forensic analysis</span></span>

<span data-ttu-id="7f544-110">有关详细信息，请参阅 [从 Azure 信息保护记录日志和分析保护使用情况](https://docs.microsoft.com/azure/information-protection/log-analyze-usage)。</span><span class="sxs-lookup"><span data-stu-id="7f544-110">For more information, see [Logging and analyzing the protection usage from Azure Information Protection](https://docs.microsoft.com/azure/information-protection/log-analyze-usage).</span></span>

<span data-ttu-id="7f544-111">有关客户端使用情况记录的信息，请参阅 [管理员指南： Azure 信息保护客户端文件和客户端使用情况日志记录](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-files-and-logging)。</span><span class="sxs-lookup"><span data-stu-id="7f544-111">For information about client usage logging, see [Admin Guide: Azure Information Protection client files and client usage logging](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-files-and-logging).</span></span>

<span data-ttu-id="7f544-112">有关额外详细信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="7f544-112">For additional information, see:</span></span>

- <span data-ttu-id="7f544-113">[Azure 信息保护要求](https://docs.microsoft.com/azure/information-protection/get-started/requirements)。</span><span class="sxs-lookup"><span data-stu-id="7f544-113">[Azure Information Protection requirements](https://docs.microsoft.com/azure/information-protection/get-started/requirements).</span></span>
    
- <span data-ttu-id="7f544-114">[教程：配置 Azure 信息保护策略设置和创建新标签](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)。</span><span class="sxs-lookup"><span data-stu-id="7f544-114">[Tutorial: Configure Azure Information Protection policy settings and create a new label](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial).</span></span>