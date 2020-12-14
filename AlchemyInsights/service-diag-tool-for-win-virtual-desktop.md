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
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Windows 虚拟桌面的服务诊断工具

Windows 虚拟桌面 (WVD) 提供了一个诊断工具，使管理员可以通过单个界面识别错误。 只要分配有 WVD 角色的某人使用 WVD，此工具就会记录诊断相关信息。 每个日志都包含有关活动所涉及的 WVD 角色的信息、会话期间出现的错误消息以及租户和用户相关信息。 可以将 Azure Log Analytics 配置为捕获诊断工具创建的活动日志。 操作步骤如下：

1. 使用 Azure 门户或 [Azure](https://go.microsoft.com/fwlink/?linkid=2129500) [PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501)创建 Log Analytics 工作区。
1. [将 Windows 计算机连接到 Azure Monitor。](https://go.microsoft.com/fwlink/?linkid=2129913) 获取工作区的工作区 ID 和主键。 安装向导需要此信息来正确配置代理并确保它可以与 Azure Monitor 通信。
1. [将诊断数据推送到工作区](https://go.microsoft.com/fwlink/?linkid=2128284)。 可以将诊断数据从 WVD 租户推送到工作区的 Log Analytics。
1. [识别并诊断与](https://go.microsoft.com/fwlink/?linkid=2128338) WVD 相关的内部或外部问题。

若要了解有关为 WVD 配置服务诊断工具的信息，请参阅"对诊断功能[使用日志分析"。](https://go.microsoft.com/fwlink/?linkid=2128084)
