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
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49652124"
---
# <a name="device-in-pending-state"></a>设备挂起状态

**先决条件：**

1. 如果是首次设置设备注册，请确保已查看 [Azure Active Directory (Azure AD) ](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) 中的设备管理简介，该简介将指导你如何获取受 Azure AD 控制的设备。
2. 如果你直接将设备注册到 Azure AD 并注册到 Intune 中，你将需要确保你已配置[Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support)并首先获得许可[](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support)。
3. 确保你有权在 Azure AD 和本地 AD 中执行操作。 只有 Azure AD 中的全局管理员可以管理设备注册的设置。 此外，如果要在本地 Active Directory 中设置自动注册，则需要是 Active Directory 和 AD FS (管理员（如果适用) ）。

混合 Azure AD 加入注册过程要求设备位于企业网络中。 它还适用于 VPN，但需要注意一些问题。 我们听到客户需要协助解决远程工作环境下的混合 Azure AD 加入注册过程。

**云身份验证环境 (Azure AD 密码哈希同步或传递身份验证)**

此注册流也称为"同步加入"。

以下是注册过程中所发生事情的细目：

1. Windows 10 在用户登录 (SCP) 发现服务连接点。

    1. 设备首先尝试从注册表中的客户端 SCP 检索租户信息 [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]。 有关详细信息，请参阅 [文档](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)。
    1. 如果失败，设备会与本地 Active Directory 通信，以从 SCP 获取租户信息。 若要验证 SCP，请参阅 [本文档](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)。

    > [!NOTE]
    > 我们建议在 Active Directory 中启用 SCP，并且仅使用客户端 SCP 进行初始验证。

2. Windows 10 尝试在系统上下文中与 Azure AD 进行通信，以针对 Azure AD 自行进行身份验证。

    可以使用测试设备注册连接脚本验证设备能否访问系统帐户下的 Microsoft [资源](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0)。

3. Windows 10 生成自签名证书，并存储在本地 Active Directory 中的计算机对象下。 这需要域控制器的视线。

4. 具有证书的设备对象通过 Azure AD Connect 同步到 Azure AD。 默认情况下，同步周期是每 30 分钟一次，但它取决于 Azure AD Connect 的配置。 有关详细信息，请参阅 [本文档](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)。

5. 在此阶段，你应该能够在 Azure 门户的设备边栏选项卡下看到主题设备处于"挂起"状态。

6. 下次用户登录到 Windows 10 时，将完成注册。

    > [!NOTE]
    > 如果你使用 VPN 并且注销/登录终止了域连接，你可以手动触发注册。 为此，请执行以下操作：
    >
    > 在本地 `dsregcmd /join` 管理员提示或通过 PSExec 远程向电脑发出。
    >
    > 例如：`PsExec -s \\win10client01 cmd, dsregcmd /join`

有关 Azure Active Directory 设备注册的常见问题，请参阅 [设备常见问题](https://docs.microsoft.com/azure/active-directory/devices/faq)解答。
