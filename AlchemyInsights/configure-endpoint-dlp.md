---
title: 配置终结点 DLP
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
- "6108"
- "3200001"
ms.openlocfilehash: 039c8f78c5896b66eab5763fb0bbddd3f0b06f2d
ms.sourcegitcommit: 1dada930649a2625eb6d15910b2bfd5e1e00e5b6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/03/2020
ms.locfileid: "46543744"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="9bb2f-102">配置终结点 DLP</span><span class="sxs-lookup"><span data-stu-id="9bb2f-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="9bb2f-103">Microsoft Endpoint DLP 允许你将 DLP 保护和监视功能扩展至 Windows 10 设备上的敏感信息。</span><span class="sxs-lookup"><span data-stu-id="9bb2f-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="9bb2f-104">设备载入到设备管理后，你可以创建 DLP 策略，以便强制执行对项目的保护操作。</span><span class="sxs-lookup"><span data-stu-id="9bb2f-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="9bb2f-105">活动资源管理器可用于监视敏感项目的活动。</span><span class="sxs-lookup"><span data-stu-id="9bb2f-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="9bb2f-106">有关详细信息，请参阅 [将设备载入设备管理](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)。</span><span class="sxs-lookup"><span data-stu-id="9bb2f-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="9bb2f-107">开始使用终结点 DLP：</span><span class="sxs-lookup"><span data-stu-id="9bb2f-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="9bb2f-108">确保拥有相应的 SKU/订阅许可。</span><span class="sxs-lookup"><span data-stu-id="9bb2f-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="9bb2f-109">有关详细信息，请参阅 [SKU/订阅许可](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing)。</span><span class="sxs-lookup"><span data-stu-id="9bb2f-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="9bb2f-110">检查启用设备管理、访问载入页面，或打开/关闭设备监视所需的权限。</span><span class="sxs-lookup"><span data-stu-id="9bb2f-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="9bb2f-111">有关详细信息，请参阅 [权限](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions)。</span><span class="sxs-lookup"><span data-stu-id="9bb2f-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="9bb2f-112">按照载入设备步骤，将设备载入进设备管理。</span><span class="sxs-lookup"><span data-stu-id="9bb2f-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="9bb2f-113">如果你缺少“M365 合规性**设置**”下的“设备载入（预览版）”选项，请确认你有上面所述的相应许可证和权限。</span><span class="sxs-lookup"><span data-stu-id="9bb2f-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="9bb2f-114">有关详细信息，请参阅 [载入设备](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices)。</span><span class="sxs-lookup"><span data-stu-id="9bb2f-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="9bb2f-115">创建 DLP 策略来保护你的敏感项目。</span><span class="sxs-lookup"><span data-stu-id="9bb2f-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="9bb2f-116">有关信息，请参阅[终结点 DLP 策略方案](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios)。</span><span class="sxs-lookup"><span data-stu-id="9bb2f-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="9bb2f-117">有关 Microsoft 终结点 DLP 的更多详细信息，请参阅 [了解 Microsoft 365 终结点数据丢失防护（预览版）](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about)。</span><span class="sxs-lookup"><span data-stu-id="9bb2f-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>