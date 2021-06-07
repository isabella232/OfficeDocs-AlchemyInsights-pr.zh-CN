---
title: Microsoft Defender for Endpoint on Microsoft 上的性能问题
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52783416"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a><span data-ttu-id="27b7c-102">Microsoft Defender for Endpoint on Microsoft 上的性能问题</span><span class="sxs-lookup"><span data-stu-id="27b7c-102">Performance issues for Microsoft Defender for Endpoint on Linux</span></span>

<span data-ttu-id="27b7c-103">本文将引导你完成识别适用于 Microsoft Defender for Endpoint（Microsoft Defender for Endpoint）性能问题的步骤。</span><span class="sxs-lookup"><span data-stu-id="27b7c-103">This article guides you through the steps of identifying performance issues for Microsoft Defender for Endpoint on Linux.</span></span>

<span data-ttu-id="27b7c-104">首先验证您遇到的问题是否已通过[最新版本](/microsoft-365/security/defender-endpoint/linux-whatsnew)解决，这一点很重要。</span><span class="sxs-lookup"><span data-stu-id="27b7c-104">It's important to first verify that the problem you're experiencing is resolved with the [latest version](/microsoft-365/security/defender-endpoint/linux-whatsnew).</span></span> 

<span data-ttu-id="27b7c-105">若要开始调查，请参阅 [Linux上的 Microsoft Defender for Endpoint 性能问题的疑难](/microsoft-365/security/defender-endpoint/linux-support-perf)。</span><span class="sxs-lookup"><span data-stu-id="27b7c-105">To start your investigation, see [Troubleshoot performance issues for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).</span></span>

## <a name="exclusions"></a><span data-ttu-id="27b7c-106">排除项</span><span class="sxs-lookup"><span data-stu-id="27b7c-106">Exclusions</span></span>

<span data-ttu-id="27b7c-107">排除可帮助缓解性能问题。</span><span class="sxs-lookup"><span data-stu-id="27b7c-107">Exclusions can help to mitigate performance issues.</span></span> <span data-ttu-id="27b7c-108">开始之前应检查排除项，以便已知且记录任何其他风险。</span><span class="sxs-lookup"><span data-stu-id="27b7c-108">Review your exclusions before you begin so any additional risk is known and documented.</span></span>

<span data-ttu-id="27b7c-109">有关详细信息，请参阅 [并验证 Microsoft Defender for Endpoint 在Linux上的排除](/microsoft-365/security/defender-endpoint/linux-exclusions)。</span><span class="sxs-lookup"><span data-stu-id="27b7c-109">For more information, see [Configure and validate exclusions for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).</span></span>

<span data-ttu-id="27b7c-110">如果有多个要排除的文件和文件夹且它们均位于同一个挂载上，排除挂载项可能更简单。</span><span class="sxs-lookup"><span data-stu-id="27b7c-110">When you have multiple files & folders to exclude and they're all on the same mountpoint, it might be easier to exclude the mountpoint.</span></span> <span data-ttu-id="27b7c-111">从 2 月 101.22.80 版开始，可以排除整个挂载。</span><span class="sxs-lookup"><span data-stu-id="27b7c-111">Starting with February release 101.22.80, you can exclude an entire mountpoint.</span></span>

<span data-ttu-id="27b7c-112">例如，如果 /mnt/backup 是一个挂载项，则可通过运行以下命令将 /mnt/backup 添加到排除列表：</span><span class="sxs-lookup"><span data-stu-id="27b7c-112">For example, if /mnt/backup is a mountpoint, you can add /mnt/backup to the exclude list by running this command:</span></span>

`$ mdatp exclusion folder add –path /mnt/backup`

<span data-ttu-id="27b7c-113">**注意**：添加排除会增加未检测到恶意软件的风险，应谨慎处理和实施。</span><span class="sxs-lookup"><span data-stu-id="27b7c-113">**Note**: Adding exclusions increases the risk of malware not being detected and should be handled and implemented with care.</span></span>

## <a name="need-help"></a><span data-ttu-id="27b7c-114">需要帮助？</span><span class="sxs-lookup"><span data-stu-id="27b7c-114">Need Help?</span></span>

<span data-ttu-id="27b7c-115">要以最高效的方式提供帮助，请打开支持案例前收集诊断数据。</span><span class="sxs-lookup"><span data-stu-id="27b7c-115">To assist you in the most efficient way, collect the diagnostic data before opening a support case.</span></span>
