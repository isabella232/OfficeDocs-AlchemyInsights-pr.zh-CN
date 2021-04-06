---
title: Windows Virtual Desktop 的服务诊断工具
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/05/2021
ms.locfileid: "51590266"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="b5d22-102">Windows Virtual Desktop 的服务诊断工具</span><span class="sxs-lookup"><span data-stu-id="b5d22-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="b5d22-103">Windows Virtual Desktop （WVD） 提供一种诊断工具，使管理员能够通过单个界面识别错误。</span><span class="sxs-lookup"><span data-stu-id="b5d22-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="b5d22-104">每当分配了 WVD 角色的某人使用 WVD 时，此工具将记录与诊断相关的信息。</span><span class="sxs-lookup"><span data-stu-id="b5d22-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="b5d22-105">每个日志都包含有关活动所涉及的 WVD 角色的信息、会话期间出现的错误消息，以及租户和用户的信息。</span><span class="sxs-lookup"><span data-stu-id="b5d22-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="b5d22-106">Azure 日志分析可以配置为通过执行下列步骤捕获由诊断工具创建的活动日志：</span><span class="sxs-lookup"><span data-stu-id="b5d22-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool by following these steps:</span></span>

1. <span data-ttu-id="b5d22-107">使用 Azure 门户或 Azure PowerShell [或](https://go.microsoft.com/fwlink/?linkid=2129500) 创建 [分析](https://go.microsoft.com/fwlink/?linkid=2129501)。</span><span class="sxs-lookup"><span data-stu-id="b5d22-107">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>

1. <span data-ttu-id="b5d22-108">[将 Windows 计算机连接到 Azure 监视器](https://go.microsoft.com/fwlink/?linkid=2129913)。</span><span class="sxs-lookup"><span data-stu-id="b5d22-108">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="b5d22-109">获取工作区 ID 和工作区的主键。</span><span class="sxs-lookup"><span data-stu-id="b5d22-109">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="b5d22-110">设置向导需要此信息来正确配置代理，并确保其可以使用 Azure 监视器进行通信。</span><span class="sxs-lookup"><span data-stu-id="b5d22-110">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>

1. <span data-ttu-id="b5d22-111">[将诊断数据推送到工作区](https://go.microsoft.com/fwlink/?linkid=2128284)。</span><span class="sxs-lookup"><span data-stu-id="b5d22-111">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="b5d22-112">您可以将诊断数据从 WVD 租户推送到工作区的日志分析。</span><span class="sxs-lookup"><span data-stu-id="b5d22-112">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>

1. <span data-ttu-id="b5d22-113">[识别和诊断](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) WVD 相关的内部或外部问题。</span><span class="sxs-lookup"><span data-stu-id="b5d22-113">[Identify and diagnose](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) issues that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="b5d22-114">若要深入了解如何配置 WVD 的服务诊断工具，请参阅将日志分析用于诊断功能。</span><span class="sxs-lookup"><span data-stu-id="b5d22-114">To learn more about configuring the service diagnostics tool for WVD, see Use Log Analytics for the diagnostics feature.</span></span>