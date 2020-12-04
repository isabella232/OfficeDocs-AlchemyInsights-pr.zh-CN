---
title: 解决 PRT 问题
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571820"
---
# <a name="troubleshoot-prt-issue"></a>解决 PRT 问题

若要使任何设备完成身份验证，必须完全注册并处于正常状态，并且能够 (PRT) 中获取主刷新令牌。

混合 Azure AD 加入注册过程需要设备位于企业网络上。 它还通过 VPN 工作，但有一些注意事项。 我们已听取客户需要在远程工作环境中对混合 Azure AD 加入注册过程进行故障排除的帮助。 下面是在注册过程中对 "盖子" 下发生的事情的细目。

**使用 Azure AD 密码哈希同步或传递身份验证 (云身份验证环境)**

此注册流程也称为 "同步加入"。

1. Windows 10 在用户登录设备时发现 SCP 记录。
    1. 设备首先尝试从注册表 [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD] 中的客户端 SCP 检索租户信息。 有关详细信息，请参阅本 [文档](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)。
    2. 如果失败，则设备与本地 Active Directory (AD) 通信，以从服务连接点 (SCP) 获取租户信息。 若要验证 SCP，请参阅本 [文档](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)。 

> [!NOTE]
> 我们建议在 AD 中启用 SCP，并且仅使用客户端 SCP 进行初始验证。

2. Windows 10 尝试在系统上下文中与 Azure AD 进行通信，以针对 Azure AD 进行身份验证。 您可以使用测试设备注册连接脚本来验证设备是否可以访问系统帐户下的 Microsoft 资源。

3. Windows 10 生成自签名证书，并将其存储在本地 AD 中的计算机对象下。 这需要向域控制器进行实时滚动。

4. 具有证书的设备对象通过 Azure AD Connect 同步到 Azure AD。 默认情况下，同步周期每30分钟一次，但具体取决于 Azure AD Connect 的配置。 有关详细信息，请参阅本 [文档](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)。

5. 在此阶段，您应能够在 Azure 门户的设备刀片下的 "挂起" 状态中查看主题设备。

6. 在下一个用户登录到 Windows 10 时，将完成注册。 

> [!NOTE]
> 如果你在 VPN 上且注销登录过程终止了域连接，则可以手动触发注册：
 1. 在管理员提示符处或远程通过 PSExec 将 dsregcmd/join 从本地发出到你的电脑。 例如，PsExec-s \\ win10client01 cmd，dsregcmd/join

 2. 有关混合加入问题的更多详细信息，请参阅 [设备问题故障排除](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344)。
