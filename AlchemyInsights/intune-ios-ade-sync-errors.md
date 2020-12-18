---
title: Apple 自动设备注册同步错误
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/17/2020
ms.locfileid: "49707858"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="5ec07-102">Apple 自动设备注册同步错误</span><span class="sxs-lookup"><span data-stu-id="5ec07-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="5ec07-103">"我们检测到你拥有一个或多个 ADE/DEP 令牌，这些令牌的状态为错误。</span><span class="sxs-lookup"><span data-stu-id="5ec07-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="5ec07-104">在解决每个受影响的令牌的错误状态之前，ADE 功能将不能用于同一个"。</span><span class="sxs-lookup"><span data-stu-id="5ec07-104">Until the error state is resolved for each affected token, the ADE functionality will not work for the same”.</span></span>

<span data-ttu-id="5ec07-105">此错误可能以多种方式显示，包括：</span><span class="sxs-lookup"><span data-stu-id="5ec07-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="5ec07-106">设备可能无法从 ABM/ASM 同步到 Intune</span><span class="sxs-lookup"><span data-stu-id="5ec07-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="5ec07-107">注册配置文件分配可能失败</span><span class="sxs-lookup"><span data-stu-id="5ec07-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="5ec07-108">设备可能无法成功完成 ADE 注册</span><span class="sxs-lookup"><span data-stu-id="5ec07-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="5ec07-109">在设备 > **注册设备 > Apple** 注册 > 注册计划令牌下检查 Intune 控制台中报告的同步错误，并查看以下文档以查看任何可能的修正：</span><span class="sxs-lookup"><span data-stu-id="5ec07-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens** and review the following documentation to see any potential remediation:</span></span>

[<span data-ttu-id="5ec07-110">iOS/iPadOS 和 macOS 自动设备注册令牌的 ABM/ASM 同步错误</span><span class="sxs-lookup"><span data-stu-id="5ec07-110">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
