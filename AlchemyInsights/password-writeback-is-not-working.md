---
title: 密码写回无法工作
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
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/12/2021
ms.locfileid: "50232663"
---
# <a name="password-writeback-is-not-working"></a>密码写回无法工作

**我在配置密码写回时遇到问题**

- 密码写回是一项高级功能。
- 确保您了解许可要求：
  - 必须在组织中分配至少一个许可证
  - **仅云用户** - 任何 Office 365 (O365) 付费 SKU 或 Azure AD Basic
  - **云和/或** 本地用户 - Azure AD Premium P1 或 P2、企业移动性 + 安全性 (EMS) 或安全生产企业 (SPE) 
    - 若要了解有关许可要求的信息，请参阅[Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)自助服务密码重置的许可要求
- 您至少有一个管理员帐户和一个具有相应许可证之一的测试用户帐户。
- 必须将 Azure AD Connect 连接到主域控制器仿真器，密码写回才能工作。 可以通过右键单击 Active Directory 同步连接器的属性，然后选择配置目录分区，将 Azure AD Connect 配置为使用主 **域控制器**。 从该位置查找 **域控制器连接设置** 部分，并选中标题仅使用首选域控制器 **的框**。
  > [!NOTE]
  > 如果首选 DC 不是 PDC 仿真器，Azure AD Connect 仍将联系 PDC 进行密码写回。
- 已在租户中配置和启用密码重置。 有关详细信息，请参阅"[允许用户重置其 Azure AD 密码"。](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)
- 确保用于启用密码写回的管理员帐户是在 Azure AD (本地 AD 帐户创建的云管理员) 
- 你拥有运行 Windows Server 2008 R2、Windows Server 2012 或 Windows Server 2012 R2 的单个或多林 AD 本地部署，并安装了最新的 Service Pack
- 已安装 Azure AD Connect 工具，并且已准备 AD 环境以同步到云。 在测试密码写回之前，请确保首先从 Azure AD Connect 中的 AD 和 Azure AD 完成完全导入和完全同步。
- 若要了解更多信息，请参阅如何在 Azure [AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)中执行完全同步和完全导入

**密码写回连接出现问题**

1. 下载并启用 [最新版本的 Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)
2. 防火墙配置：Azure AD Connect (1.1.443 及) 将需要出 **站 HTTPS** 访问权限：
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. 允许空闲连接至少保留 2-3 分钟

**我仍遇到密码写回问题**

- 如果仍有问题，请尝试在 Azure AD Connect 工具中禁用和重新启用密码写回服务
- 若要了解更多信息，请参阅如何 [禁用和重新启用密码写回](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
