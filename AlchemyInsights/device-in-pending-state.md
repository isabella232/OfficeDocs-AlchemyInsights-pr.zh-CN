---
title: 设备挂起状态
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: 7d8a55f8c9a9fc30c653152c2f1b185874cea3ee
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330362"
---
# <a name="device-in-pending-state"></a>设备挂起状态

**先决条件：**

1. 如果是首次设置设备注册，请确保已查看[Azure Active Directory (Azure AD) ](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support)中的设备管理简介，该简介将指导你如何在 Azure AD 控制下获取设备。
2. 如果你直接将设备注册到 Azure AD 中，并注册到 Intune 中，则需要确保你已配置[Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support)并首先获得[](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support)许可。
3. 确保你有权在 Azure AD 和本地 AD 中执行操作。 只有 Azure AD 中的全局管理员可管理设备注册的设置。 此外，若要在本地 Active Directory 中设置自动注册，需成为 Active Directory 和 AD FS 的管理员 (如果适用)。

混合 Azure AD 加入注册过程要求设备位于企业网络上。 它还通过 VPN 运行，但有一些注意事项。 我们收到客户在远程工作环境中需要有关混合 Azure AD 加入注册过程疑难解答的帮助。

**云身份验证 (Azure AD 密码哈希同步或传递身份验证)**

此注册流也称为"同步加入"。

下面是注册过程中所发生事情的细目：

1. Windows 10登录到设备时 (SCP) 服务连接点记录。

    1. 设备首先尝试从注册表 [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD] 中的客户端 SCP 检索租户信息。 有关详细信息， [请参阅文档](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)。
    1. 如果失败，设备会与本地 Active Directory 通信，以从 SCP 获取租户信息。 若要验证 SCP，请参阅 [此文档](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)。

    **注意**：我们建议在 Active Directory 中启用 SCP，并且仅使用客户端 SCP 进行初始验证。

2. Windows 10尝试在系统上下文下与 Azure AD 进行通信，以针对 Azure AD 自行进行身份验证。

    可以使用测试设备注册连接脚本 验证设备能否访问系统帐户下的 Microsoft [资源](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0)。

3. Windows 10生成自签名证书，并存储在本地 Active Directory 中的计算机对象下。 这需要域控制器的"看到线"。

4. 具有证书的设备对象通过 Azure AD 连接。 默认情况下，同步周期每 30 分钟一次，但具体取决于 Azure AD 连接。 有关详细信息，请参阅此 [文档](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)。

5. 在此阶段，你应该能够在 Azure 门户的设备边栏选项卡下看到处于"挂起"状态的主题设备。

6. 下次用户登录到 Windows 10时，将完成注册。

    **注意**：如果你使用 VPN 并且注销/登录终止了域连接，你可以手动触发注册。 为此，请执行以下操作：
    
    通过管理员 `dsregcmd /join` 提示在本地或通过 PSExec 远程向电脑发出问题。\
    例如：`PsExec -s \\win10client01 cmd, dsregcmd /join`

有关设备注册Azure Active Directory常见问题，请参阅[设备常见问题](https://docs.microsoft.com/azure/active-directory/devices/faq)。
