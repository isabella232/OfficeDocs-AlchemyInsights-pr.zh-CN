---
title: EndPoint Manager - 安全基准
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2021
ms.locfileid: "51408740"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="b6ff2-102">EndPoint Manager - 安全基准</span><span class="sxs-lookup"><span data-stu-id="b6ff2-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="b6ff2-103">安全基准是预配置的 Windows 设置组，可帮助应用相关安全团队推荐的安全设置。</span><span class="sxs-lookup"><span data-stu-id="b6ff2-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="b6ff2-104">这些比较基准可以自定义，以仅提供所需的设置和值。</span><span class="sxs-lookup"><span data-stu-id="b6ff2-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="b6ff2-105">有关安全基线详细信息，请参阅使用 [在 Intune 设备中配置 Windows 10](https://docs.microsoft.com/mem/intune/protect/security-baselines)。</span><span class="sxs-lookup"><span data-stu-id="b6ff2-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="b6ff2-106">这些产品当前有比较基准：</span><span class="sxs-lookup"><span data-stu-id="b6ff2-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="b6ff2-107">Windows MDM 安全设置</span><span class="sxs-lookup"><span data-stu-id="b6ff2-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="b6ff2-108">适用于 EndPoint 安全性的 Microsoft Defender</span><span class="sxs-lookup"><span data-stu-id="b6ff2-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="b6ff2-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="b6ff2-109">Microsoft Edge</span></span>

<span data-ttu-id="b6ff2-110">每个基准会定期更新，并按增量版本发布。</span><span class="sxs-lookup"><span data-stu-id="b6ff2-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="b6ff2-111">每个版本都会添加或删除早期版本中的设置，以确保基线满足当前指导。</span><span class="sxs-lookup"><span data-stu-id="b6ff2-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="b6ff2-112">终结点安全中的安全基线控制台通过显示版本更改来比较不同版本。</span><span class="sxs-lookup"><span data-stu-id="b6ff2-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="b6ff2-113">有关如何最有效地更改所部署的基线版本的指导，请参阅 [Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure)。</span><span class="sxs-lookup"><span data-stu-id="b6ff2-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="b6ff2-114">部署安全基准后，可监视部署状态并按设备查看设置。</span><span class="sxs-lookup"><span data-stu-id="b6ff2-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="b6ff2-115">**注意：** 基准的报告数据可能需要多达 24 小时才能从初始部署显示到设备，而进一步更新最多需要 6 小时。</span><span class="sxs-lookup"><span data-stu-id="b6ff2-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="b6ff2-116">基线设置不应用最常见的原因是在不同的配置文件中使用的设置相同。</span><span class="sxs-lookup"><span data-stu-id="b6ff2-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="b6ff2-117">可通过从"安全基线"配置文件的"设备状态"节点中选择特定设备来调查此方案。</span><span class="sxs-lookup"><span data-stu-id="b6ff2-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="b6ff2-118">有关详细信息，请参阅 [解决安全基线](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines)。</span><span class="sxs-lookup"><span data-stu-id="b6ff2-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>