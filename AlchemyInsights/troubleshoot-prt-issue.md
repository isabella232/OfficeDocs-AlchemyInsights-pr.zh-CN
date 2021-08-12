---
title: PRT 问题疑难解答
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
ms.openlocfilehash: fd285d1158d7b358e4c698cf6014422cc2fb536e1fbdf98630bebda359f9c553
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972706"
---
# <a name="troubleshoot-prt-issue"></a>PRT 问题疑难解答

若要使任何设备完成身份验证，设备必须完全注册且状态良好，并且能够获取 PRT (主刷新) 。

混合 Azure AD 加入注册过程要求设备位于企业网络中。 它还通过 VPN 运行，但有一些注意事项。 我们收到客户在远程工作环境中需要解决混合 Azure AD 加入注册过程的帮助。 下面细目了注册过程中"底层"发生的情况。

**使用 Azure AD (哈希同步或传递身份验证方法的云身份验证)**

此注册流也称为"同步加入"。

1. Windows 10登录到设备时发现 SCP 记录。
    1. 设备首先尝试从注册表 [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD] 中的客户端 SCP 检索租户信息。 有关详细信息，请参阅此[文档](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)。
    2. 如果失败，设备会与本地 Active Directory (AD) 通信，以从 SCP 服务连接点 (租户) 。 若要验证 SCP，请参阅此 [文档](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)。 

> [!NOTE]
> 我们建议在 AD 中启用 SCP，并且仅使用客户端 SCP 进行初始验证。

2. Windows 10尝试在系统上下文下与 Azure AD 进行通信，以针对 Azure AD 自行进行身份验证。 可以使用测试设备注册连接脚本验证设备能否访问系统帐户下的 Microsoft 资源。

3. Windows 10生成自签名证书，并在本地 AD 中的计算机对象下存储该证书。 这需要域控制器的"看到线"。

4. 具有证书的设备对象通过 Azure AD 连接 同步到 Azure AD。 默认情况下，同步周期每 30 分钟一次，但具体取决于 Azure AD 连接。 有关详细信息，请参阅此 [文档](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)。

5. 在此阶段，你应该能够在 Azure 门户的设备边栏选项卡下看到主题设备处于"挂起"状态。

6. 下次用户登录到 Windows 10时，将完成注册。 

> [!NOTE]
> 如果你使用 VPN 并且注销登录过程终止了域连接，你可以手动触发注册：
 1. 在管理员提示符上本地发出 dsregcmd /join，或通过 PSExec 远程将 dsregcmd /join 发至电脑。 例如，PsExec -s \\ win10client01 cmd、 dsregcmd /join

 2. 有关混合加入问题的更多详细信息，请参阅 [设备问题疑难解答](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344)。
