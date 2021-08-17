---
title: Windows Virtual Desktop 的服务诊断工具
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
ms.openlocfilehash: 58688e3216ba6777b1a4f76095bd39c81a2d2a8294e06b6bc61c7134f6d589f9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052376"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Windows Virtual Desktop 的服务诊断工具

Windows Virtual Desktop （WVD） 提供一种诊断工具，使管理员能够通过单个界面识别错误。 每当分配了 WVD 角色的某人使用 WVD 时，此工具将记录与诊断相关的信息。 每个日志都包含有关活动所涉及的 WVD 角色的信息、会话期间出现的错误消息，以及租户和用户的信息。 可以将 Azure Log Analytics 配置为捕获诊断工具创建的活动日志。 操作步骤如下：

1. 使用 Azure 门户或 Azure PowerShell [或](https://go.microsoft.com/fwlink/?linkid=2129500) 创建 [分析](https://go.microsoft.com/fwlink/?linkid=2129501)。
1. [将 Windows 计算机连接到 Azure 监视器](https://go.microsoft.com/fwlink/?linkid=2129913)。 获取工作区 ID 和工作区的主键。 设置向导需要此信息来正确配置代理，并确保其可以使用 Azure 监视器进行通信。
1. [将诊断数据推送到工作区](https://go.microsoft.com/fwlink/?linkid=2128284)。 您可以将诊断数据从 WVD 租户推送到工作区的日志分析。
1. [确定和诊断与](https://go.microsoft.com/fwlink/?linkid=2128338) WVD 相关的内部或外部问题。

若要了解有关为 WVD 配置服务诊断工具的信息，请参阅对诊断功能[使用 Log Analytics。](https://go.microsoft.com/fwlink/?linkid=2128084)
