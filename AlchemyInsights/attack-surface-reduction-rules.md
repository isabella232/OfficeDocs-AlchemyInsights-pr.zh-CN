---
title: 攻击面减少规则
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
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2021
ms.locfileid: "52651477"
---
# <a name="attack-surface-reduction-rules"></a><span data-ttu-id="8f9f8-102">攻击面减少规则</span><span class="sxs-lookup"><span data-stu-id="8f9f8-102">Attack surface reduction rules</span></span>

<span data-ttu-id="8f9f8-103">排除文件或文件夹可以严重削弱攻击面减少规则提供的保护。</span><span class="sxs-lookup"><span data-stu-id="8f9f8-103">Excluding files or folders can severely reduce the protection provided by attack surface reduction rules.</span></span> <span data-ttu-id="8f9f8-104">允许本将由规则阻止的文件运行，并且不会记录任何报告或事件。</span><span class="sxs-lookup"><span data-stu-id="8f9f8-104">Files that would have been blocked by a rule are allowed to run, and no report or event is recorded.</span></span> <span data-ttu-id="8f9f8-105">排除应用于允许排除的所有规则。</span><span class="sxs-lookup"><span data-stu-id="8f9f8-105">An exclusion applies to all rules that allow exclusions.</span></span>

<span data-ttu-id="8f9f8-106">ASR 排除使用与 Microsoft Defender 防病毒排除相同的语法。</span><span class="sxs-lookup"><span data-stu-id="8f9f8-106">ASR exclusions use the same syntax as Microsoft Defender Antivirus exclusions.</span></span> <span data-ttu-id="8f9f8-107">有关详细信息，请参阅 [配置和验证 Microsoft Defender 防病毒扫描的排除](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus)。</span><span class="sxs-lookup"><span data-stu-id="8f9f8-107">For details, see [Configure and validate exclusions for Microsoft Defender Antivirus scans](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span></span> <span data-ttu-id="8f9f8-108">若要避免问题，请查看 [定义排除时要避免的常见错误](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus)。</span><span class="sxs-lookup"><span data-stu-id="8f9f8-108">To avoid problems, review [Common mistakes to avoid when defining exclusions](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="8f9f8-109">并非所有 ASR 规则都支持排除。</span><span class="sxs-lookup"><span data-stu-id="8f9f8-109">Not all ASR rules support exclusions.</span></span> <span data-ttu-id="8f9f8-110">要验证规则是否支持排除，请参阅表 [攻击面减少规则](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)。</span><span class="sxs-lookup"><span data-stu-id="8f9f8-110">To validate if your rule supports exclusions, see the table [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

## <a name="attack-surface-reduction-rules"></a><span data-ttu-id="8f9f8-111">攻击面减少规则</span><span class="sxs-lookup"><span data-stu-id="8f9f8-111">Attack surface reduction rules</span></span>

<span data-ttu-id="8f9f8-112">组织攻击面包括攻击者可能攻击组织设备或网络的所有位置。</span><span class="sxs-lookup"><span data-stu-id="8f9f8-112">Your organization attack surface includes all the places where an attacker could compromise organization devices or networks.</span></span> <span data-ttu-id="8f9f8-113">减少攻击面意味着保护组织设备和网络，减少攻击者执行攻击的方式。</span><span class="sxs-lookup"><span data-stu-id="8f9f8-113">Reducing your attack surface means protecting the organization devices and network, which leaves attackers with fewer ways to perform attacks.</span></span> <span data-ttu-id="8f9f8-114">在 Microsoft Defender for Endpoint 中配置攻击面减少规则会有助于此。</span><span class="sxs-lookup"><span data-stu-id="8f9f8-114">Configuring attack surface reduction rules in Microsoft Defender for Endpoint can help.</span></span>

<span data-ttu-id="8f9f8-115">有关详细信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="8f9f8-115">For more information, see:</span></span>

- [<span data-ttu-id="8f9f8-116">将 ASR 规则 GUID 映射到名称</span><span class="sxs-lookup"><span data-stu-id="8f9f8-116">Map ASR rule GUID to name</span></span>](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- <span data-ttu-id="8f9f8-117">ASR 规则要求：</span><span class="sxs-lookup"><span data-stu-id="8f9f8-117">ASR rules requirements:</span></span>
    - [<span data-ttu-id="8f9f8-118">Windows 10 专业版，版本 1709 或更高版本</span><span class="sxs-lookup"><span data-stu-id="8f9f8-118">Windows 10 Pro, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="8f9f8-119">Windows 10 企业版，版本 1709 或更高版本</span><span class="sxs-lookup"><span data-stu-id="8f9f8-119">Windows 10 Enterprise, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="8f9f8-120">Windows Server 版本 1803（半年度频道）或更高版本</span><span class="sxs-lookup"><span data-stu-id="8f9f8-120">Windows Server, version 1803 (Semi-Annual Channel) or later</span></span>](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a><span data-ttu-id="8f9f8-121">识别正确排除以应用</span><span class="sxs-lookup"><span data-stu-id="8f9f8-121">Identify the correct exclusion to apply</span></span>

1. <span data-ttu-id="8f9f8-122">在 Microsoft-Windows-Windows Defender/Operational.log 中查找 eventID 1121 或 1122。</span><span class="sxs-lookup"><span data-stu-id="8f9f8-122">Look for eventID 1121 or 1122 in the Microsoft-Windows-Windows Defender/Operational log.</span></span>

1. <span data-ttu-id="8f9f8-123">评估此方案需要取消阻止的阻止方案和上下文。</span><span class="sxs-lookup"><span data-stu-id="8f9f8-123">Evaluate the block scenario and context and confirm that this scenario needs to be unblocked.</span></span>

1. <span data-ttu-id="8f9f8-124">读取事件详细信息中的路径值，即定义该排除的值。</span><span class="sxs-lookup"><span data-stu-id="8f9f8-124">Read the Path value in the event details, which is the value that defines the exclusion.</span></span>
    - <span data-ttu-id="8f9f8-125">尽可能严格地进行排除。</span><span class="sxs-lookup"><span data-stu-id="8f9f8-125">Make the exclusion as strict as possible.</span></span>
    - <span data-ttu-id="8f9f8-126">按需应用通配符（例如替换用户变量）。</span><span class="sxs-lookup"><span data-stu-id="8f9f8-126">Apply a wildcard where needed (for example, replace User variable).</span></span>

1. <span data-ttu-id="8f9f8-127">根据部署需求应用排除。</span><span class="sxs-lookup"><span data-stu-id="8f9f8-127">Apply the exclusion according to your deployment needs.</span></span> <span data-ttu-id="8f9f8-128">有关详细信息，请参阅 [自定义攻击面减少规则](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction)。</span><span class="sxs-lookup"><span data-stu-id="8f9f8-128">For details, see [Customize attack surface reduction rules](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span></span>

## <a name="exclusion-is-not-honored"></a><span data-ttu-id="8f9f8-129">不尊重排除</span><span class="sxs-lookup"><span data-stu-id="8f9f8-129">Exclusion is not honored</span></span>

1. <span data-ttu-id="8f9f8-130">确定规则是否支持排除。</span><span class="sxs-lookup"><span data-stu-id="8f9f8-130">Determine whether the rule support exclusions.</span></span> <span data-ttu-id="8f9f8-131">有关详细信息，请参阅 [自定义减少攻击面规则](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)。</span><span class="sxs-lookup"><span data-stu-id="8f9f8-131">For details, see [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

1. <span data-ttu-id="8f9f8-132">查看已应用的排除，并通过事件数据验证键入错误或解读错误的通配符。</span><span class="sxs-lookup"><span data-stu-id="8f9f8-132">Review the exclusions applied and verify with the event data for typos or misinterpreted wildcards.</span></span> <span data-ttu-id="8f9f8-133">有关详细信息，请参阅 [支持的排除类型](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span><span class="sxs-lookup"><span data-stu-id="8f9f8-133">For more info, see [Supported exclusion types](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span></span>

1. <span data-ttu-id="8f9f8-134">如果规则影响过大，请考虑将规则移动（或移回）到审核模式，以执行进一步验证。</span><span class="sxs-lookup"><span data-stu-id="8f9f8-134">if the impact of the rule it too high, consider moving the rule (back) to Audit mode to perform further validation.</span></span> <span data-ttu-id="8f9f8-135">有关详细信息，请参阅 [测试 Microsoft Defender for Endpoint 功能在审核模式下的工作情况](/microsoft-365/security/defender-endpoint/audit-windows-defender)。</span><span class="sxs-lookup"><span data-stu-id="8f9f8-135">For details, see [Test how Microsoft Defender for Endpoint features work in audit mode](/microsoft-365/security/defender-endpoint/audit-windows-defender).</span></span>

1. <span data-ttu-id="8f9f8-136">通过使用此命令收集支持数据，以打开支持案例：</span><span class="sxs-lookup"><span data-stu-id="8f9f8-136">Collect support data to open a support case by using this command:</span></span>
    
   <span data-ttu-id="8f9f8-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span><span class="sxs-lookup"><span data-stu-id="8f9f8-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span></span>

    <span data-ttu-id="8f9f8-138">有关详细信息，请参阅 [将计算机载入到 Microsoft Defender for Endpoint 时出现问题](issues-with-onboarding-machines.md)。</span><span class="sxs-lookup"><span data-stu-id="8f9f8-138">For more information, see [Issues with onboarding machines to Microsoft Defender for Endpoints](issues-with-onboarding-machines.md).</span></span>
