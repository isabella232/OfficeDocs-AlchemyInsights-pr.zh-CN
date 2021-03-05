---
title: Apple 自动设备注册同步错误
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448912"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="c3103-102">Apple 自动设备注册同步错误</span><span class="sxs-lookup"><span data-stu-id="c3103-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="c3103-103">"我们检测到你拥有一个或多个 ADE/DEP 令牌，这些令牌在错误状态中。</span><span class="sxs-lookup"><span data-stu-id="c3103-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="c3103-104">在解决每个受影响的令牌的错误状态之前，ADE 功能不会像预期一样工作。"。</span><span class="sxs-lookup"><span data-stu-id="c3103-104">Until the error state is resolved for each affected token, the ADE functionality will not work as expected.”.</span></span>

<span data-ttu-id="c3103-105">此错误可能以多种方式显示，包括：</span><span class="sxs-lookup"><span data-stu-id="c3103-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="c3103-106">设备可能无法从 ABM/ASM 同步到 Intune</span><span class="sxs-lookup"><span data-stu-id="c3103-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="c3103-107">注册配置文件分配可能失败</span><span class="sxs-lookup"><span data-stu-id="c3103-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="c3103-108">设备可能无法成功完成 ADE 注册</span><span class="sxs-lookup"><span data-stu-id="c3103-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="c3103-109">检查 Intune 控制台中"设备注册设备>注册设备> Apple 注册> **注册计划令牌** 下报告的同步错误。</span><span class="sxs-lookup"><span data-stu-id="c3103-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens**.</span></span>

<span data-ttu-id="c3103-110">同步错误的最常见原因之一是当前令牌过期。</span><span class="sxs-lookup"><span data-stu-id="c3103-110">One of the most common causes of sync error is expiration of the current token.</span></span> <span data-ttu-id="c3103-111">在许多情况下，受影响令牌的续订将解决问题。</span><span class="sxs-lookup"><span data-stu-id="c3103-111">In many cases,renewal of the affected token will resolve the issue.</span></span>

<span data-ttu-id="c3103-112">如果一个或多个令牌已过期，请参阅以下文档，以帮助你根据情况续订它们：</span><span class="sxs-lookup"><span data-stu-id="c3103-112">If one or more of your tokens has expired,  see the following documentation to help you renew them as appropriate:</span></span>

[<span data-ttu-id="c3103-113">续订自动设备注册令牌</span><span class="sxs-lookup"><span data-stu-id="c3103-113">Renew an Automated Device Enrollment token</span></span>](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

<span data-ttu-id="c3103-114">此外，还可以参阅以下文档，了解可能导致令牌同步失败的其他错误的潜在修正：</span><span class="sxs-lookup"><span data-stu-id="c3103-114">In addition, you can see the following documentation to see potential remediations for other errors causing token synchronization failures:</span></span>

[<span data-ttu-id="c3103-115">iOS/iPadOS 和 macOS 自动设备注册令牌的 ABM/ASM 同步错误</span><span class="sxs-lookup"><span data-stu-id="c3103-115">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[<span data-ttu-id="c3103-116">iOS/iPadOS 和 macOS 自动设备注册令牌的 ABM/ASM 同步错误</span><span class="sxs-lookup"><span data-stu-id="c3103-116">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
