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
ms.openlocfilehash: 679dea6d488cf74f51baee2b3b498dc64b95530e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324913"
---
# <a name="password-writeback-is-not-working"></a>密码写回无法工作

**我在配置密码写回时遇到问题**

- 密码写回是一项高级功能。
- 确保您了解许可要求：
  - 必须在组织中至少分配一个许可证
  - **仅云用户**- Office 365 (O365) 付费 SKU 或 Azure AD Basic
  - **云和/或本地用户**- Azure AD Premium P1 P2、企业移动性 + 安全性 (EMS) 或 Secure Productive Enterprise (SPE) 
    - 若要了解有关许可要求的信息，请参阅[Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)自助服务密码重置的许可要求
- 您至少有一个管理员帐户和一个测试用户帐户具有一个相应的许可证。
- 必须将 Azure AD 连接连接到主域控制器Emulator密码写回才能正常工作。 你可以将 Azure AD 连接配置为使用主域控制器，方法是右键单击 Active  Directory 同步连接器的属性，然后选择配置 **目录分区**。 从该位置查找 **域控制器连接设置** 部分，并选中标题为"仅使用首选域控制器 **"的框**。
    **注意**：如果首选 DC 不是 PDC 仿真器，Azure AD 连接仍将联系 PDC 进行密码写回。
- 已在租户中配置并启用密码重置。 有关详细信息，请参阅允许用户 [重置其 Azure AD 密码](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)。
- 确保用于启用密码写回的管理员帐户是在 Azure AD 中创建的云 (帐户，而不是在本地 AD) 
- 您具有运行 Windows Server 2008 R2、Windows Server 2012 或 Windows Server 2012 R2 的单林或多林 AD 本地部署，并安装了最新的 Service Pack
- 已安装 Azure AD 连接工具，并且已准备 AD 环境以与云同步。 在测试密码写回之前，请确保首先从 Azure AD 连接 中的 AD 和 Azure AD 完成完全导入和完全连接。
- 若要了解更多信息，请参阅如何在 Azure [AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)服务中执行完全同步和完全连接

**密码写回连接出现问题**

1. 下载并启用最新版[Azure AD 连接](https://www.microsoft.com/download/details.aspx?id=47594)
2. 防火墙配置：连接 1.1.443 (及以上的 Azure AD) 工具将需要 **出站 HTTPS** 访问权限：
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. 允许空闲连接至少保留 2-3 分钟

**我仍遇到密码写回问题**

- 如果仍有困难，请尝试在 Azure AD 连接工具中禁用和重新启用密码写回服务
- 若要了解更多信息，请参阅 [如何禁用和重新启用密码写回](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
