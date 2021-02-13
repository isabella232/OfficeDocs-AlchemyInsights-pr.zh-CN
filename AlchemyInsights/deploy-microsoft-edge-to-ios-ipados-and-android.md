---
title: 将 Microsoft Edge 部署到 iOS、iPadOS 和 Android
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8241"
- "9004604"
ms.openlocfilehash: 524e87ab57e29823361053093708c83831f19687
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50177987"
---
# <a name="deploy-microsoft-edge-to-ios-ipados-and-android"></a><span data-ttu-id="a8d52-102">将 Microsoft Edge 部署到 iOS、iPadOS 和 Android</span><span class="sxs-lookup"><span data-stu-id="a8d52-102">Deploy Microsoft Edge to iOS, iPadOS, and Android</span></span>

<span data-ttu-id="a8d52-103">下面总结的指导方案将帮助你将 Microsoft Edge 分配给 iOS、iPadOS 和 Android 设备的用户。</span><span class="sxs-lookup"><span data-stu-id="a8d52-103">The guided scenario summarized below will help you assign Microsoft Edge to users of iOS, iPadOS, and Android devices.</span></span>

> [!NOTE]
> <span data-ttu-id="a8d52-104">如果你阻止用户注册移动设备，此指导方案将不起作用，并且用户需要自行安装 Microsoft Edge。</span><span class="sxs-lookup"><span data-stu-id="a8d52-104">If you blocked users from enrolling mobile devices, this guided scenario won't work and the users will need to install Microsoft Edge on their own.</span></span>

<span data-ttu-id="a8d52-105">指导方案涉及以下步骤：</span><span class="sxs-lookup"><span data-stu-id="a8d52-105">The guided scenario involves the following steps:</span></span>

1. [<span data-ttu-id="a8d52-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="a8d52-106">Prerequisites</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#prerequisites)
2. [<span data-ttu-id="a8d52-107">简介</span><span class="sxs-lookup"><span data-stu-id="a8d52-107">Introduction</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-1---introduction)
3. [<span data-ttu-id="a8d52-108">基本信息</span><span class="sxs-lookup"><span data-stu-id="a8d52-108">Basics</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-2---basics)
4. [<span data-ttu-id="a8d52-109">配置</span><span class="sxs-lookup"><span data-stu-id="a8d52-109">Configuration</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-3---configuration)
5. [<span data-ttu-id="a8d52-110">作业</span><span class="sxs-lookup"><span data-stu-id="a8d52-110">Assignments</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-4---assignments)
6. [<span data-ttu-id="a8d52-111">查看和创建</span><span class="sxs-lookup"><span data-stu-id="a8d52-111">Review and creation</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-5---review--create)

<span data-ttu-id="a8d52-112">完成指导方案中的步骤后，Microsoft Intune 策略将启用 Microsoft Edge for Business 的以下功能：</span><span class="sxs-lookup"><span data-stu-id="a8d52-112">After you complete the steps in the guided scenario, Microsoft Intune policies will enable the following features of Microsoft Edge for business:</span></span>

- <span data-ttu-id="a8d52-113">双重身份</span><span class="sxs-lookup"><span data-stu-id="a8d52-113">Dual identity</span></span>
- <span data-ttu-id="a8d52-114">与 Microsoft Intune 应用保护策略集成</span><span class="sxs-lookup"><span data-stu-id="a8d52-114">Integration with Microsoft Intune app protection policy</span></span>
- <span data-ttu-id="a8d52-115">与 Azure Active Directory 应用程序代理集成</span><span class="sxs-lookup"><span data-stu-id="a8d52-115">Integration with Azure Active Directory Application Proxy</span></span>
- <span data-ttu-id="a8d52-116">托管收藏夹和主页快捷方式</span><span class="sxs-lookup"><span data-stu-id="a8d52-116">Managed favorites and home page shortcuts</span></span>
