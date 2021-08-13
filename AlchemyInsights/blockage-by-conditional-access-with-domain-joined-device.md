---
title: 由于使用已加入域的设备被条件访问阻止
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: f0d092dfbc805b1e4fa7d26803227118b39ecacca9fa330bb5de8458d4aa0f57
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53950286"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a>由于使用已加入域的设备被条件访问阻止

**强烈建议使用的工具**

[设备注册疑难解答工具](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - 一可帮助解决最常见设备注册问题的工具。

[测试设备注册连接脚本](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - 此脚本有助于确保设备可以访问系统帐户下的设备注册终结点。

[Azure AD 设备清理脚本](https://github.com/mzmaili/AzureADDeviceCleanup) - 此脚本可用于查找和管理环境中过时的设备。

以下是为什么有条件访问可能会使已加入域的设备（混合 Azure AD）失败的一些常见原因。

1. **设备上没有 Azure AD PRT** - 需要确保设备具有 Azure AD 主刷新令牌 (PRT)。有关 PRT 的详细信息，请参阅此 [文档](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)。

若要验证是否具有 Azure AD PRT，可以在设备上运行 `dsregcmd/status` 命令，并验证 “AzureAdPrt” 是否等于 “YES”。

如果"AzureAdPrt"为"NO"，请检查以下内容：

- **是否拥有含有 AD FS 的联合环境，并且访问用户的家庭网络**：在这种情况下，请确保从 Extranet 可以访问 "usernamemixed"终结点。 如果 AD FS 位于 VPN 后，请确保用户连接到 VPN，然后重新登录到设备。 有关详细信息，请参阅此[文档](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains)。

- **设备的 TPM 是否有故障，因此无法验证设备**：检查 "tpm.msc" 以查看 TPM 的状态是否为“就绪”。 如果不是，请运行 `dsregcmd/leave`，然后让设备重新加入 Azure AD。 之后再重试。 有关详细信息，请参阅此[文档](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)。

- **你使用的是第三方标识提供程序，此提供程序不支持 WS-Trust 协议**。 如我们的文档所述，在这种情况下，混合使用 Azure AD 的混合设备无法正常工作。 请与标识提供者合作以获取支持。

2. **用户使用的是没有 Windows 10 帐户的 Chrome 浏览器** 或 **Office 扩展 Chrome 不会自动在加入 AAD 的设备或加入 AAD 的混合设备上自动使用 PRT**：这会导致任何基于设备的条件访问策略失败，并显示“未注册的设备”错误消息。 如果要正确使用 Chrome 浏览器，必须通过 SCCM 或 Intune 安装 “Windows 10 帐户”或“ 用户 Chrome 浏览器的 Office 扩展”。 有关详细信息，请参阅此[文档](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)。

如果无法远程推送扩展，请通知用户手动安装上述扩展之一，以访问为基于设备的条件访问提供支持的应用程序。有关详细信息，请参阅此[文档](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites)。

3. **此设备已正确建立混合 Azure AD 联接，但是由于 Azure AD Connect 或 Azure 门户中的同步更改而无意中将其删除或禁用**：如果发生这种情况，即使 "AzureAdJoined" 和 "PRT" 状态在设备上显示为有效，此设备对象也不再被识别为完全连接的设备。

若要解决此问题，请在受影响的设备上运行 `dsregcmd/leave`，让它们重新加入 Azure AD。有关详细信息，请参阅此[文档](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices)。

> [!NOTE]
> 如果设备是 Windows 10 1809 更新版本，且具有VPN / Cloud 代理，并且看到 "AzureAdPrt" 状态的问题或任何具有SSO问题的应用程序（即使拥有PRT，也无法连接到邮箱），确保拥有此修补程序 [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2)或四月累积更新 [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6)，以防止这些计算机上的 PRT 失败。

















