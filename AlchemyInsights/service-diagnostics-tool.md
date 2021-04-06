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
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Windows Virtual Desktop 的服务诊断工具

Windows Virtual Desktop （WVD） 提供一种诊断工具，使管理员能够通过单个界面识别错误。 每当分配了 WVD 角色的某人使用 WVD 时，此工具将记录与诊断相关的信息。 每个日志都包含有关活动所涉及的 WVD 角色的信息、会话期间出现的错误消息，以及租户和用户的信息。 Azure 日志分析可以配置为通过执行下列步骤捕获由诊断工具创建的活动日志：

1. 使用 Azure 门户或 Azure PowerShell [或](https://go.microsoft.com/fwlink/?linkid=2129500) 创建 [分析](https://go.microsoft.com/fwlink/?linkid=2129501)。

1. [将 Windows 计算机连接到 Azure 监视器](https://go.microsoft.com/fwlink/?linkid=2129913)。 获取工作区 ID 和工作区的主键。 设置向导需要此信息来正确配置代理，并确保其可以使用 Azure 监视器进行通信。

1. [将诊断数据推送到工作区](https://go.microsoft.com/fwlink/?linkid=2128284)。 您可以将诊断数据从 WVD 租户推送到工作区的日志分析。

1. [识别和诊断](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) WVD 相关的内部或外部问题。

若要深入了解如何配置 WVD 的服务诊断工具，请参阅将日志分析用于诊断功能。