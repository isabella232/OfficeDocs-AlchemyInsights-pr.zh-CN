---
title: 评估现有浏览器环境和浏览器需求
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
- "9141"
- "9005291"
ms.openlocfilehash: 5b03d188aa78be83928cf262f1d86f3f933c85ab
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2021
ms.locfileid: "50529893"
---
# <a name="evaluate-your-existing-browser-environment-and-define-goals"></a><span data-ttu-id="f3e60-102">评估现有浏览器环境和浏览器需求</span><span class="sxs-lookup"><span data-stu-id="f3e60-102">Evaluate your existing browser environment and define goals</span></span>

<span data-ttu-id="f3e60-103">请花些时间来了解当前的浏览器状态和项目远景，以确保所有项目利益相关方都保持一致并努力达到相同的结果。</span><span class="sxs-lookup"><span data-stu-id="f3e60-103">Taking time to understand your current browser state and project vision ensures all project stakeholders are aligned and are working toward the same goal.</span></span> <span data-ttu-id="f3e60-104">请按以下步骤操作：</span><span class="sxs-lookup"><span data-stu-id="f3e60-104">Follow these steps:</span></span>

1. <span data-ttu-id="f3e60-105">定义当前状态。</span><span class="sxs-lookup"><span data-stu-id="f3e60-105">Define your current state.</span></span> <span data-ttu-id="f3e60-106">比如以下几种情况：</span><span class="sxs-lookup"><span data-stu-id="f3e60-106">Consider the following:</span></span>
- <span data-ttu-id="f3e60-107">当前在环境中部署了哪些浏览器？</span><span class="sxs-lookup"><span data-stu-id="f3e60-107">Which browsers are currently deployed in your environment?</span></span>
- <span data-ttu-id="f3e60-108">哪个浏览器被设置为默认浏览器？</span><span class="sxs-lookup"><span data-stu-id="f3e60-108">Which browser is set as the default browser?</span></span>
- <span data-ttu-id="f3e60-109">是否需要将 Internet Explorer 用于某些应用？</span><span class="sxs-lookup"><span data-stu-id="f3e60-109">Do you need to use Internet Explorer for some of your apps?</span></span>
- <span data-ttu-id="f3e60-110">现在你是否使用企业模式站点列表配置 Internet Explorer？</span><span class="sxs-lookup"><span data-stu-id="f3e60-110">Do you use an Enterprise Mode Site List to configure Internet Explorer today?</span></span>
- <span data-ttu-id="f3e60-111">你的环境支持哪些操作系统平台，例如 Windows 10 和 macOS？</span><span class="sxs-lookup"><span data-stu-id="f3e60-111">Which OS platforms, such as Windows 10 and macOS, does your environment support?</span></span>
- <span data-ttu-id="f3e60-112">你使用哪些管理工具进行浏览器管理？</span><span class="sxs-lookup"><span data-stu-id="f3e60-112">Which management tools do you use for browser management?</span></span>
- <span data-ttu-id="f3e60-113">谁负责浏览器配置和管理？</span><span class="sxs-lookup"><span data-stu-id="f3e60-113">Who's responsible for browser configuration and management?</span></span>
- <span data-ttu-id="f3e60-114">验证浏览器兼容性的过程是什么？</span><span class="sxs-lookup"><span data-stu-id="f3e60-114">What's the process for validating browser compatibility?</span></span>
2. <span data-ttu-id="f3e60-115">定义部署目标。</span><span class="sxs-lookup"><span data-stu-id="f3e60-115">Define the goals for your deployment.</span></span> <span data-ttu-id="f3e60-116">请记住以下事项：</span><span class="sxs-lookup"><span data-stu-id="f3e60-116">Keep the following things in mind:</span></span>
- <span data-ttu-id="f3e60-117">是否要将 Microsoft Edge [为默认浏览器](https://docs.microsoft.com/DeployEdge/edge-default-browser)？</span><span class="sxs-lookup"><span data-stu-id="f3e60-117">Do you want to [set Microsoft Edge as your default browser](https://docs.microsoft.com/DeployEdge/edge-default-browser)?</span></span>
- <span data-ttu-id="f3e60-118">是希望隐藏旧版 Microsoft Edge 还是希望 [保留其可供用户使用](https://docs.microsoft.com/DeployEdge/microsoft-edge-sysupdate-access-old-edge)？</span><span class="sxs-lookup"><span data-stu-id="f3e60-118">Do you want to hide the legacy version of Microsoft Edge or do you want to [leave it available for users](https://docs.microsoft.com/DeployEdge/microsoft-edge-sysupdate-access-old-edge)?</span></span>
- <span data-ttu-id="f3e60-119">如何配置 [Microsoft Edge](https://docs.microsoft.com/DeployEdge/configure-microsoft-edge)？</span><span class="sxs-lookup"><span data-stu-id="f3e60-119">How will you [configure Microsoft Edge](https://docs.microsoft.com/DeployEdge/configure-microsoft-edge)?</span></span>
- <span data-ttu-id="f3e60-120">初始部署过程中配置哪些功能至关重要？</span><span class="sxs-lookup"><span data-stu-id="f3e60-120">What features are critical to configure as part of your initial deployment?</span></span>
- <span data-ttu-id="f3e60-121">解决任何已确定的兼容性或配置问题的过程是什么？</span><span class="sxs-lookup"><span data-stu-id="f3e60-121">What is the process for addressing any identified compatibility or configuration issues?</span></span>
3. <span data-ttu-id="f3e60-122">了解可能希望使用的功能的先决条件，如：</span><span class="sxs-lookup"><span data-stu-id="f3e60-122">Understand the prerequisites for features you might want to use, such as:</span></span>
- [<span data-ttu-id="f3e60-123">Windows Defender 应用程序防护</span><span class="sxs-lookup"><span data-stu-id="f3e60-123">Windows Defender Application Guard</span></span>](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-application-guard/reqs-md-app-guard)
- [<span data-ttu-id="f3e60-124">Internet Explorer 模式</span><span class="sxs-lookup"><span data-stu-id="f3e60-124">Internet Explorer mode</span></span>](https://docs.microsoft.com/DeployEdge/edge-ie-mode)
- [<span data-ttu-id="f3e60-125">身份验证和同步</span><span class="sxs-lookup"><span data-stu-id="f3e60-125">Authentication and sync</span></span>](https://docs.microsoft.com/DeployEdge/microsoft-edge-security-identity)

<span data-ttu-id="f3e60-126">完成这些步骤后，即可开始制定部署策略。</span><span class="sxs-lookup"><span data-stu-id="f3e60-126">After you complete these steps, you're ready to start planning your deployment strategy.</span></span>
