---
title: 指示器使用 Edge 浏览器不起作用
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2021
ms.locfileid: "52651481"
---
# <a name="indicators-dont-work-using-edge-browser"></a><span data-ttu-id="5811e-102">指示器使用 Edge 浏览器不起作用</span><span class="sxs-lookup"><span data-stu-id="5811e-102">Indicators don't work using Edge browser</span></span>

<span data-ttu-id="5811e-103">创建指示器后，Edge （Smartscreen） 不授予其荣誉。</span><span class="sxs-lookup"><span data-stu-id="5811e-103">After you created an Indicator, it's not honored by Edge (Smartscreen).</span></span> <span data-ttu-id="5811e-104">有关详细信息，请参阅 [IP 和 URL/域标记](/microsoft-365/security/defender-endpoint/indicator-ip-domain)。</span><span class="sxs-lookup"><span data-stu-id="5811e-104">For more information, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>

## <a name="step-1-ensure-the-following"></a><span data-ttu-id="5811e-105">步骤 1：确保以下内容</span><span class="sxs-lookup"><span data-stu-id="5811e-105">Step 1: Ensure the following</span></span>

- <span data-ttu-id="5811e-106">验证指示器是否正确（IP/URL 中无拼写错误，操作正确，RBAC 组正确）。</span><span class="sxs-lookup"><span data-stu-id="5811e-106">Verify that the indicator is correct (no typos in IP/URL, correct action, the correct RBAC groups).</span></span>
- <span data-ttu-id="5811e-107">创建指示器后至少等待 2 小时，考虑任何可能延迟。</span><span class="sxs-lookup"><span data-stu-id="5811e-107">Wait the minimum 2 hours after creating the indicator to take into account any possible latency.</span></span>
- <span data-ttu-id="5811e-108">确认系统已载入 Microsoft Defender for Endpoint。</span><span class="sxs-lookup"><span data-stu-id="5811e-108">Confirm that the system(s) are onboarded to Microsoft Defender for Endpoint.</span></span>
- <span data-ttu-id="5811e-109">验证系统能否与云进行通信。</span><span class="sxs-lookup"><span data-stu-id="5811e-109">Verify that system(s) can communicate with the Cloud.</span></span>
- <span data-ttu-id="5811e-110">通过转到[测试站点](https://demo.smartscreen.msft.net)，验证Smartscreen是否已启用并可以访问。</span><span class="sxs-lookup"><span data-stu-id="5811e-110">Verify that Smartscreen is enabled and reachable by going to the [test site](https://demo.smartscreen.msft.net).</span></span>

## <a name="step-2-troubleshoot-the-potential-issue"></a><span data-ttu-id="5811e-111">步骤 2：解决潜在问题</span><span class="sxs-lookup"><span data-stu-id="5811e-111">Step 2: Troubleshoot the potential issue</span></span>

- <span data-ttu-id="5811e-112">请确保客户端满足要求。</span><span class="sxs-lookup"><span data-stu-id="5811e-112">Make sure the client meets the requirements.</span></span> <span data-ttu-id="5811e-113">有关详细信息，请参阅 [创建 IP 和 URL/域指示器](/microsoft-365/security/defender-endpoint/indicator-ip-domain)。</span><span class="sxs-lookup"><span data-stu-id="5811e-113">For details, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>
- <span data-ttu-id="5811e-114">请确保正在运行最新版本的 Edge 浏览器。</span><span class="sxs-lookup"><span data-stu-id="5811e-114">Make sure you're running the latest version of the Edge browser.</span></span> <span data-ttu-id="5811e-115">若要了解最新版本，请参阅 [了解你拥有哪个版本的 Microsoft Edge](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb)。</span><span class="sxs-lookup"><span data-stu-id="5811e-115">To find out the latest version, see [Find out which version of Microsoft Edge you have](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span></span>
- <span data-ttu-id="5811e-116">重启 Edge 浏览器。</span><span class="sxs-lookup"><span data-stu-id="5811e-116">Restart the Edge browser.</span></span>
- <span data-ttu-id="5811e-117">导航到已设置指示器的网站。</span><span class="sxs-lookup"><span data-stu-id="5811e-117">Navigate to the site for which you have setup an indicator.</span></span> <span data-ttu-id="5811e-118">如果网站未按预期显示，请继续执行步骤 3。</span><span class="sxs-lookup"><span data-stu-id="5811e-118">If the site does not appear as expected, continue to Step 3.</span></span> 

## <a name="step-3-collect-data"></a><span data-ttu-id="5811e-119">步骤 3：收集数据</span><span class="sxs-lookup"><span data-stu-id="5811e-119">Step 3: Collect data</span></span>

- <span data-ttu-id="5811e-120">收集 **MDEClientAnalyzer** 诊断数据。</span><span class="sxs-lookup"><span data-stu-id="5811e-120">Collect **MDEClientAnalyzer** diagnostic data.</span></span> <span data-ttu-id="5811e-121">有关说明，请参阅 [将计算机载入到 Microsoft Defender for Endpoint](issues-with-onboarding-machines.md)。</span><span class="sxs-lookup"><span data-stu-id="5811e-121">For instructions, see [Issues with onboarding machines to Microsoft Defender for Endpoint](issues-with-onboarding-machines.md).</span></span>
- <span data-ttu-id="5811e-122">如果你习惯安装和收集 Fiddler 跟踪，请参阅 [Telerik Fiddler](http://www.telerik.com/fiddler)。</span><span class="sxs-lookup"><span data-stu-id="5811e-122">If you are comfortable installing and collecting a Fiddler trace, see [Telerik Fiddler](http://www.telerik.com/fiddler).</span></span>
- <span data-ttu-id="5811e-123">如果希望从 Microsoft 支持人员获得指导，请选择下面的"支持"图标打开支持案例。</span><span class="sxs-lookup"><span data-stu-id="5811e-123">If you prefer guidance from Microsoft Support, select the Support icon below to open a support case.</span></span>
