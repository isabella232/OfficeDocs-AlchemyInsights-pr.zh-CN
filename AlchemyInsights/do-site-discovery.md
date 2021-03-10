---
title: 进行站点发现
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2021
ms.locfileid: "50529192"
---
# <a name="do-site-discovery"></a><span data-ttu-id="e20a8-102">进行站点发现</span><span class="sxs-lookup"><span data-stu-id="e20a8-102">Do site discovery</span></span>

<span data-ttu-id="e20a8-103">如果你的组织仍在使用旧版 Web 应用程序和计划以使用 Internet Explorer 模式（大多数客户都采用此模式），则你应该执行一些附加网站发现。</span><span class="sxs-lookup"><span data-stu-id="e20a8-103">If your organization still uses legacy web applications and plans to use Internet Explorer mode (which most customers do), then you should do some additional site discovery.</span></span>

<span data-ttu-id="e20a8-104">**你已部署早期版本的 Microsoft Edge**</span><span class="sxs-lookup"><span data-stu-id="e20a8-104">**You've already deployed an older version of Microsoft Edge**</span></span>

<span data-ttu-id="e20a8-105">如果你已配置你的企业网站列表以适用于旧版本的 Microsoft Edge，则你的网站发现将几乎完成。</span><span class="sxs-lookup"><span data-stu-id="e20a8-105">If you've already configured your Enterprise Site List to work for the legacy version of Microsoft Edge, then your site discovery is almost done.</span></span> <span data-ttu-id="e20a8-106">你可能需要做的一件事是添加非特定语言的网站。</span><span class="sxs-lookup"><span data-stu-id="e20a8-106">The one thing you might need to do is add neutral sites.</span></span>

<span data-ttu-id="e20a8-107">中性站点通常是提供单一登录 (SSO) 的站点。</span><span class="sxs-lookup"><span data-stu-id="e20a8-107">Neutral sites are typically sites that provide single sign-on (SSO).</span></span> <span data-ttu-id="e20a8-108">如果从 Microsoft Edge 中导航到中性站点，则需要保持在 Microsoft Edge 中以进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="e20a8-108">If you go to a neutral site from Microsoft Edge, then you want to stay in Microsoft Edge to authenticate.</span></span> <span data-ttu-id="e20a8-109">如果在 Internet Explorer 模式下导航到中性站点，则需要保持在 Internet Explorer 模式中以进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="e20a8-109">If you go to a neutral site in Internet Explorer mode, then you want to stay in Internet Explorer mode to authenticate.</span></span>

<span data-ttu-id="e20a8-110">标识使用的任何 SSO（或其他中性）站点，并将它们添加到企业站点列表中。</span><span class="sxs-lookup"><span data-stu-id="e20a8-110">Identify any SSO or other neutral sites that you use and add these to your Enterprise Site List.</span></span>

<span data-ttu-id="e20a8-111">**Internet Explorer 是默认浏览器**</span><span class="sxs-lookup"><span data-stu-id="e20a8-111">**Internet Explorer is your default browser**</span></span>

<span data-ttu-id="e20a8-112">如果当前仅使用 Internet Explorer，则可能不知道哪些站点已升级到新式 Web 标准，以及哪些仍需要 Internet Explorer。</span><span class="sxs-lookup"><span data-stu-id="e20a8-112">If you're only using Internet Explorer now, you might not know which sites have upgraded to modern web standards and which still require Internet Explorer.</span></span> <span data-ttu-id="e20a8-113">你需要查找这些网站并将其添加到企业网站列表，以便只为这些站点使用 Internet Explorer 模式。</span><span class="sxs-lookup"><span data-stu-id="e20a8-113">You'll want to find and add these sites to the Enterprise Site List so that you can use Internet Explorer mode only for those sites.</span></span>

> [!NOTE]
> <span data-ttu-id="e20a8-114">[企业网站发现](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) 发现可能需要 Internet Explorer 模式的网站。</span><span class="sxs-lookup"><span data-stu-id="e20a8-114">[Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) discovers sites that might need Internet Explorer mode.</span></span> <span data-ttu-id="e20a8-115">它可以在通过 Windows 10、Windows 8.1 或 Windows 7 上的 Internet Explorer 11 运行 Windows Internet Explorer 8 的计算机上收集数据。</span><span class="sxs-lookup"><span data-stu-id="e20a8-115">It can collect data on computers running Windows Internet Explorer 8 through Internet Explorer 11 on Windows 10, Windows 8.1, or Windows 7.</span></span>

<span data-ttu-id="e20a8-116">**分析数据**</span><span class="sxs-lookup"><span data-stu-id="e20a8-116">**Analyze the data**</span></span>

<span data-ttu-id="e20a8-117">收集站点数据后，我们建议采用以下 4 步过程来分析数据：</span><span class="sxs-lookup"><span data-stu-id="e20a8-117">After you've collected site data, we recommend the following four-step process to analyze the data:</span></span>
1. <span data-ttu-id="e20a8-118">依次按域和 URL 对数据进行排序。</span><span class="sxs-lookup"><span data-stu-id="e20a8-118">Sort the data by domain, and then by URL.</span></span>
2. <span data-ttu-id="e20a8-119">定义要为 Internet Explorer 模式配置的“应用”的边界。</span><span class="sxs-lookup"><span data-stu-id="e20a8-119">Define the boundaries of an app to configure for Internet Explorer mode.</span></span> <span data-ttu-id="e20a8-120">您希望包含定义应用的所有网站和 Web 控件，但不想包含额外的网站和控件。</span><span class="sxs-lookup"><span data-stu-id="e20a8-120">You want to include all the sites and web controls that define the app, but you don't want to include extra sites and controls.</span></span> <span data-ttu-id="e20a8-121">某些网站可能很简单，*https://contoso.com/app1* 而其他网站可能需要你定义多个网站和页面。</span><span class="sxs-lookup"><span data-stu-id="e20a8-121">Some sites might be as simple as *https://contoso.com/app1* while others might require you to define multiple sites and pages.</span></span>
3. <span data-ttu-id="e20a8-122">测试应用以验证它是否未在本机工作。</span><span class="sxs-lookup"><span data-stu-id="e20a8-122">Test the app to verify that it doesn't work natively.</span></span> <span data-ttu-id="e20a8-123">许多站点在检测到新式浏览器时将提供新式内容，并且仅在检测到 Internet Explorer 时才提供旧版内容。</span><span class="sxs-lookup"><span data-stu-id="e20a8-123">Many sites will offer modern content when they detect a modern browser and only offer legacy content when they detect Internet Explorer.</span></span>
4. <span data-ttu-id="e20a8-124">如果应用未通过测试，请将该应用添加到企业站点列表中。</span><span class="sxs-lookup"><span data-stu-id="e20a8-124">Add the app to your Enterprise Site List if it fails testing.</span></span>

> [!NOTE]
> <span data-ttu-id="e20a8-125">作为最佳做法，请将构成应用的所有站点归为一组。</span><span class="sxs-lookup"><span data-stu-id="e20a8-125">As a best practice, group all of the sites that comprise an app.</span></span> <span data-ttu-id="e20a8-126">这样，当升级应用时，可以更轻松地从 Internet Explorer 模式中删除整个站点并开始将新式浏览器用于该应用。</span><span class="sxs-lookup"><span data-stu-id="e20a8-126">This way, when you upgrade an app, it's easier to remove the entire site from Internet Explorer mode and start using a modern browser for that app.</span></span>

<span data-ttu-id="e20a8-127">完成网站发现并分析数据后，即可开始查看频道策略。</span><span class="sxs-lookup"><span data-stu-id="e20a8-127">Once you're done with site discovery and you've analyzed the data, you're ready to start looking at your channel strategy.</span></span>

