---
title: 执行应用兼容性测试
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
- "9138"
- "9005291"
ms.openlocfilehash: 9a6a9ea3587a851ecf842588ab73421590ce2431
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2021
ms.locfileid: "50529896"
---
# <a name="do-app-compatibility-testing"></a><span data-ttu-id="fd3b0-102">执行应用兼容性测试</span><span class="sxs-lookup"><span data-stu-id="fd3b0-102">Do app compatibility testing</span></span>

<span data-ttu-id="fd3b0-103">Microsoft Edge 的应用程序兼容性非常高。</span><span class="sxs-lookup"><span data-stu-id="fd3b0-103">Application compatibility for Microsoft Edge is extremely high.</span></span> <span data-ttu-id="fd3b0-104">实际上，Microsoft 会承诺以下兼容性，这一点非常高：</span><span class="sxs-lookup"><span data-stu-id="fd3b0-104">In fact, it's so high that Microsoft provides the following compatibility promises:</span></span>
- <span data-ttu-id="fd3b0-105">如果适用于 Microsoft Edge 45 和早期版本，它将适用于 Microsoft Edge 77 和更高版本。</span><span class="sxs-lookup"><span data-stu-id="fd3b0-105">If it works on Microsoft Edge 45 and earlier versions, it will work on Microsoft Edge 77 and later versions.</span></span>
- <span data-ttu-id="fd3b0-106">如果适用于 Internet Explorer，那么将在 Internet Explorer 模式下适用于 Microsoft Edge。</span><span class="sxs-lookup"><span data-stu-id="fd3b0-106">If it works on Internet Explorer, it will work on Microsoft Edge in Internet Explorer mode.</span></span>
- <span data-ttu-id="fd3b0-107">如果适用于 Google Chrome，则将适用于 Microsoft Edge。</span><span class="sxs-lookup"><span data-stu-id="fd3b0-107">If it works on Google Chrome, it will work on Microsoft Edge.</span></span>

<span data-ttu-id="fd3b0-108">如果你有一个不满足此承诺的应用程序，则我们将支持通过 Microsoft App 使用"保证" [修复](https://www.microsoft.com/fasttrack/microsoft-365/app-assure)。</span><span class="sxs-lookup"><span data-stu-id="fd3b0-108">If you have an application where we don't meet this promise, then we stand behind the promise to fix it with [Microsoft App Assure](https://www.microsoft.com/fasttrack/microsoft-365/app-assure).</span></span>

<span data-ttu-id="fd3b0-109">尽管有此承诺，但我们知道许多组织必须验证某些应用程序的合规性或风险管理原因。</span><span class="sxs-lookup"><span data-stu-id="fd3b0-109">Despite this promise, we know that many organizations must validate some applications for compliance or risk-management reasons.</span></span> <span data-ttu-id="fd3b0-110">尽管我们希望简单直接地测试应用，但此过程务必要做到严格有序。</span><span class="sxs-lookup"><span data-stu-id="fd3b0-110">Even though we expect this to be very straightforward, it's important to be organized and rigorous in app testing.</span></span>

<span data-ttu-id="fd3b0-111">有两种方法可以执行应用兼容性测试：</span><span class="sxs-lookup"><span data-stu-id="fd3b0-111">There are two ways to do app compatibility testing:</span></span>

- <span data-ttu-id="fd3b0-112">**实验室测试**：根据特定的配置，在紧密控制的环境中测试应用程序。</span><span class="sxs-lookup"><span data-stu-id="fd3b0-112">**Lab testing**: Applications are tested in a tightly controlled environment with specific configurations.</span></span>
- <span data-ttu-id="fd3b0-113">**试点测试**：应用程序由有限数量的用户使用其自己的设备在日常工作环境中进行测试。</span><span class="sxs-lookup"><span data-stu-id="fd3b0-113">**Pilot testing**: Applications are tested by a limited number of users in their daily work environment using their own devices.</span></span>

<span data-ttu-id="fd3b0-114">选择最适合每个应用的方法，在向整个组织推出之前进行测试。</span><span class="sxs-lookup"><span data-stu-id="fd3b0-114">Choose the method that is most appropriate for each app and do the testing prior to a launch to the entire organization.</span></span>

<span data-ttu-id="fd3b0-115">确保应用兼容后，即可将 Microsoft Edge 部署到试点组。</span><span class="sxs-lookup"><span data-stu-id="fd3b0-115">Once you've ensured that your apps are compatible, you're ready to deploy Microsoft Edge to a pilot group.</span></span>
