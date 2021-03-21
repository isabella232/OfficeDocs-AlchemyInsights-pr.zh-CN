---
title: 不同端口访问问题的诊断
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9035"
- "9005220"
ms.openlocfilehash: 3673067cad7ac55f3820422dc2ec09942c393149
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897422"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>不同端口访问问题的诊断

要解决不同端口访问问题，请执行以下步骤：

1. 从门户停止/取消分配虚拟机 (VM)，重新启动 VM，然后再次进行测试。 
2. 检查 VM 的网络设置，以确定是否有网络安全组 (NSG) 阻止了流量。 还可以使用 [Network Watcher 的 IP 流验证工具](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support)检查是否有 NSG 阻止了流量，是否有用户定义的路由 (UDR) 将流量重新路由回本地（“默认路由”0.0.0.0/0）或网络设备。
如果尝试上述步骤后仍然遇到问题，请提供要继续发送邮件的 VM 名称和 TCP 端口，以进行进一步诊断。

**推荐文档**

[通过端口 25 发送出站电子邮件的限制和建议](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)