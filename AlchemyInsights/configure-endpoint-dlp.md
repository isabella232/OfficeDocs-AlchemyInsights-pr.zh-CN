---
title: 配置终结点 DLP
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: b9369b2c2ca31f7d2fceac37ef1e2252b82e933b
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52657919"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="3a505-102">配置终结点 DLP</span><span class="sxs-lookup"><span data-stu-id="3a505-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="3a505-103">Microsoft Endpoint DLP 允许你将 DLP 保护和监视功能扩展至 Windows 10 设备上的敏感信息。</span><span class="sxs-lookup"><span data-stu-id="3a505-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="3a505-104">设备载入到设备管理后，你可以创建 DLP 策略，以便强制执行对项目的保护操作。</span><span class="sxs-lookup"><span data-stu-id="3a505-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="3a505-105">活动资源管理器可用于监视敏感项目的活动。</span><span class="sxs-lookup"><span data-stu-id="3a505-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="3a505-106">有关详细信息，请参阅 [将设备载入设备管理](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)。</span><span class="sxs-lookup"><span data-stu-id="3a505-106">For more info, see [Onboarding devices into device management](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="3a505-107">开始使用终结点 DLP：</span><span class="sxs-lookup"><span data-stu-id="3a505-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="3a505-108">确保拥有相应的 SKU/订阅许可。</span><span class="sxs-lookup"><span data-stu-id="3a505-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="3a505-109">有关详细信息，请参阅 [SKU/订阅许可](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing)。</span><span class="sxs-lookup"><span data-stu-id="3a505-109">For more info, see [SKU/subscriptions licensing](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="3a505-p103">检查启用设备管理、访问载入页面或打开/关闭设备监视所需的权限。有关详细信息，请参阅 [权限](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions)。</span><span class="sxs-lookup"><span data-stu-id="3a505-p103">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring. For more info, see [Permissions](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="3a505-112">按照载入设备步骤，将设备载入进设备管理。</span><span class="sxs-lookup"><span data-stu-id="3a505-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="3a505-113">有关详细信息，请参阅 [载入设备](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices)。</span><span class="sxs-lookup"><span data-stu-id="3a505-113">For more info, see [Onboarding devices](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="3a505-114">创建 DLP 策略来保护你的敏感项目。</span><span class="sxs-lookup"><span data-stu-id="3a505-114">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="3a505-115">有关信息，请参阅[终结点 DLP 策略方案](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios)。</span><span class="sxs-lookup"><span data-stu-id="3a505-115">For info, see [Endpoint DLP policy scenarios](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="3a505-116">有关 Microsoft 终结点 DLP 的更多详细信息，请参阅 [了解 Microsoft 365 终结点数据丢失防护（预览版）](/microsoft-365/compliance/endpoint-dlp-learn-about)。</span><span class="sxs-lookup"><span data-stu-id="3a505-116">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="3a505-117">**如需要支持，请采取以下重要数据收集步骤：**</span><span class="sxs-lookup"><span data-stu-id="3a505-117">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="3a505-118">下载 [MDATP 客户端分析器预览版](https://aka.ms/betamdatpanalyzer)。</span><span class="sxs-lookup"><span data-stu-id="3a505-118">Download [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).</span></span>
1. <span data-ttu-id="3a505-119">以管理员身份从 cmd 窗口运行该工具：</span><span class="sxs-lookup"><span data-stu-id="3a505-119">Run the tool as Admin from the cmd window:</span></span>

    <span data-ttu-id="3a505-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span><span class="sxs-lookup"><span data-stu-id="3a505-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span></span>

1. <span data-ttu-id="3a505-121">当系统提示 **输入收集跟踪的分钟数：**，输入运行方案所需的分钟数。</span><span class="sxs-lookup"><span data-stu-id="3a505-121">When prompted with **Enter the number of minutes to collect traces:**, enter the number of minutes required to run the scenario.</span></span>
1. <span data-ttu-id="3a505-122">运行场景。</span><span class="sxs-lookup"><span data-stu-id="3a505-122">Run the scenario.</span></span>

<span data-ttu-id="3a505-123">收集Zip文件输出以提供给支持代理。</span><span class="sxs-lookup"><span data-stu-id="3a505-123">Collect the Zip file output to give to the Support agent.</span></span>
