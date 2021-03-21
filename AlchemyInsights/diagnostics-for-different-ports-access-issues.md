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
# <a name="diagnostics-for-different-ports-access-issues"></a><span data-ttu-id="9df1d-102">不同端口访问问题的诊断</span><span class="sxs-lookup"><span data-stu-id="9df1d-102">Diagnostics for different ports access issues</span></span>

<span data-ttu-id="9df1d-103">要解决不同端口访问问题，请执行以下步骤：</span><span class="sxs-lookup"><span data-stu-id="9df1d-103">To resolve the different port access issues, perform the following steps:</span></span>

1. <span data-ttu-id="9df1d-104">从门户停止/取消分配虚拟机 (VM)，重新启动 VM，然后再次进行测试。</span><span class="sxs-lookup"><span data-stu-id="9df1d-104">Stop/deallocate the virtual machine (VM) from the portal, restart the VM, and test again.</span></span> 
2. <span data-ttu-id="9df1d-105">检查 VM 的网络设置，以确定是否有网络安全组 (NSG) 阻止了流量。</span><span class="sxs-lookup"><span data-stu-id="9df1d-105">Check your VM's network settings to determine if you have Network Security Groups (NSGs) blocking traffic.</span></span> <span data-ttu-id="9df1d-106">还可以使用 [Network Watcher 的 IP 流验证工具](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support)检查是否有 NSG 阻止了流量，是否有用户定义的路由 (UDR) 将流量重新路由回本地（“默认路由”0.0.0.0/0）或网络设备。</span><span class="sxs-lookup"><span data-stu-id="9df1d-106">You can also use [Network Watcher's IP flow verify tool](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) to check for NSGs blocking traffic, User-Defined Routes (UDRs) rerouting your traffic back to on-premises ('Default Route' 0.0.0.0/0), or to a network appliance.</span></span>
<span data-ttu-id="9df1d-107">如果尝试上述步骤后仍然遇到问题，请提供要继续发送邮件的 VM 名称和 TCP 端口，以进行进一步诊断。</span><span class="sxs-lookup"><span data-stu-id="9df1d-107">If you still experience issues after trying the steps above, please provide the VM name and the TCP port you are attempting to send mail on for further diagnosis.</span></span>

<span data-ttu-id="9df1d-108">**推荐文档**</span><span class="sxs-lookup"><span data-stu-id="9df1d-108">**Recommended Documents**</span></span>

[<span data-ttu-id="9df1d-109">通过端口 25 发送出站电子邮件的限制和建议</span><span class="sxs-lookup"><span data-stu-id="9df1d-109">Limitations and recommendations for sending outbound email over port 25</span></span>](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)