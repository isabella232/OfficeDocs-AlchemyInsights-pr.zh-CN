---
title: 应用程序保护策略
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 929400dcf0ca18ce8f52cb11e5c907064449480e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47716883"
---
# <a name="application-protection-policy"></a><span data-ttu-id="a82c4-102">应用程序保护策略</span><span class="sxs-lookup"><span data-stu-id="a82c4-102">Application protection policy</span></span>

<span data-ttu-id="a82c4-103">如果你不熟悉应用程序保护策略 (APP)，请查看[应用程序保护策略概述](https://docs.microsoft.com/intune/apps/app-protection-policy)。</span><span class="sxs-lookup"><span data-stu-id="a82c4-103">If you're new to Application protection policy (APP), check out the [App protection policies overview](https://docs.microsoft.com/intune/apps/app-protection-policy).</span></span>

<span data-ttu-id="a82c4-104">要开始使用 APP，请参阅[如何创建和分配应用保护策略](https://docs.microsoft.com/intune/app-protection-policies)。</span><span class="sxs-lookup"><span data-stu-id="a82c4-104">To start using APP, see [How to create and assign app protection policies](https://docs.microsoft.com/intune/app-protection-policies).</span></span>

<span data-ttu-id="a82c4-105">应用程序保护策略要求：</span><span class="sxs-lookup"><span data-stu-id="a82c4-105">Application protection policy requirements:</span></span>

- <span data-ttu-id="a82c4-106">用户拥有 Intune 或 EMS 许可证。</span><span class="sxs-lookup"><span data-stu-id="a82c4-106">User has an Intune or EMS license.</span></span>
- <span data-ttu-id="a82c4-107">用户属于应用程序保护策略的目标组。</span><span class="sxs-lookup"><span data-stu-id="a82c4-107">User belongs to a group targeted by application protection policies.</span></span>
- <span data-ttu-id="a82c4-108">只有一个企业用户登录到设备上受保护的应用程序。</span><span class="sxs-lookup"><span data-stu-id="a82c4-108">Only one corporate user is signed into protected apps on a device.</span></span>
- <span data-ttu-id="a82c4-109">应用程序已实施 [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started)。</span><span class="sxs-lookup"><span data-stu-id="a82c4-109">The application has implemented the [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span></span> <span data-ttu-id="a82c4-110">有关支持 SDK 的应用的列表，请参阅 [Microsoft Intune 的受保护应用](https://docs.microsoft.com/intune/apps-supported-intune-apps)。</span><span class="sxs-lookup"><span data-stu-id="a82c4-110">For a list of apps that support the SDK, see [Microsoft Intune protected apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span></span>

<span data-ttu-id="a82c4-111">满足上述要求的用户登录启用 Intune SDK 的应用后，将应用策略。</span><span class="sxs-lookup"><span data-stu-id="a82c4-111">Policies apply after a user who meets the above requirements signs into an Intune SDK enabled app.</span></span> <span data-ttu-id="a82c4-112">确定是否应用策略的最简单方法是要求用户在策略中设置 PIN。</span><span class="sxs-lookup"><span data-stu-id="a82c4-112">The easiest way to determine if a policy is applied is by requiring that the user set a pin in the policy.</span></span> 

<span data-ttu-id="a82c4-113">有关详细信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="a82c4-113">For more information, see:</span></span>

[<span data-ttu-id="a82c4-114">APP/MAM 常见问题疑难解答</span><span class="sxs-lookup"><span data-stu-id="a82c4-114">APP/MAM troubleshooting FAQ</span></span>](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[<span data-ttu-id="a82c4-115">如何验证应用保护策略设置</span><span class="sxs-lookup"><span data-stu-id="a82c4-115">How to validate your app protection policy setup</span></span>](https://docs.microsoft.com/intune/app-protection-policies-validate)

[<span data-ttu-id="a82c4-116">了解应用保护策略发布时间</span><span class="sxs-lookup"><span data-stu-id="a82c4-116">Understand App Protection Policy delivery timing</span></span>](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[<span data-ttu-id="a82c4-117">如何监视 Intune 应用保护策略</span><span class="sxs-lookup"><span data-stu-id="a82c4-117">How to monitor app protection policies</span></span>](https://docs.microsoft.com/intune/app-protection-policies-monitor)