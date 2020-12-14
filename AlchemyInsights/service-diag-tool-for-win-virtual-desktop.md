---
title: Windows 虚拟桌面的服务诊断工具
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/14/2020
ms.locfileid: "49665812"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="c925d-102">Windows 虚拟桌面的服务诊断工具</span><span class="sxs-lookup"><span data-stu-id="c925d-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="c925d-103">Windows 虚拟桌面 (WVD) 提供了一个诊断工具，使管理员可以通过单个界面识别错误。</span><span class="sxs-lookup"><span data-stu-id="c925d-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="c925d-104">只要分配有 WVD 角色的某人使用 WVD，此工具就会记录诊断相关信息。</span><span class="sxs-lookup"><span data-stu-id="c925d-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="c925d-105">每个日志都包含有关活动所涉及的 WVD 角色的信息、会话期间出现的错误消息以及租户和用户相关信息。</span><span class="sxs-lookup"><span data-stu-id="c925d-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="c925d-106">可以将 Azure Log Analytics 配置为捕获诊断工具创建的活动日志。</span><span class="sxs-lookup"><span data-stu-id="c925d-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool.</span></span> <span data-ttu-id="c925d-107">操作步骤如下：</span><span class="sxs-lookup"><span data-stu-id="c925d-107">Here's how:</span></span>

1. <span data-ttu-id="c925d-108">使用 Azure 门户或 [Azure](https://go.microsoft.com/fwlink/?linkid=2129500) [PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501)创建 Log Analytics 工作区。</span><span class="sxs-lookup"><span data-stu-id="c925d-108">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>
1. <span data-ttu-id="c925d-109">[将 Windows 计算机连接到 Azure Monitor。](https://go.microsoft.com/fwlink/?linkid=2129913)</span><span class="sxs-lookup"><span data-stu-id="c925d-109">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="c925d-110">获取工作区的工作区 ID 和主键。</span><span class="sxs-lookup"><span data-stu-id="c925d-110">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="c925d-111">安装向导需要此信息来正确配置代理并确保它可以与 Azure Monitor 通信。</span><span class="sxs-lookup"><span data-stu-id="c925d-111">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>
1. <span data-ttu-id="c925d-112">[将诊断数据推送到工作区](https://go.microsoft.com/fwlink/?linkid=2128284)。</span><span class="sxs-lookup"><span data-stu-id="c925d-112">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="c925d-113">可以将诊断数据从 WVD 租户推送到工作区的 Log Analytics。</span><span class="sxs-lookup"><span data-stu-id="c925d-113">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>
1. <span data-ttu-id="c925d-114">[识别并诊断与](https://go.microsoft.com/fwlink/?linkid=2128338) WVD 相关的内部或外部问题。</span><span class="sxs-lookup"><span data-stu-id="c925d-114">[Identify and diagnose issues](https://go.microsoft.com/fwlink/?linkid=2128338) that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="c925d-115">若要了解有关为 WVD 配置服务诊断工具的信息，请参阅"对诊断功能[使用日志分析"。](https://go.microsoft.com/fwlink/?linkid=2128084)</span><span class="sxs-lookup"><span data-stu-id="c925d-115">To learn more about configuring the service diagnostics tool for WVD, see [Use Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2128084).</span></span>
