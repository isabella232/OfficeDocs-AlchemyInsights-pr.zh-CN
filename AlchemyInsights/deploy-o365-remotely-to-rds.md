---
title: 部署Microsoft 365 应用版在 RDS、终端服务器或 VDI 上共享使用
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 81183cf1823480c1b15eba9ba9f519b4e3746b52
ms.sourcegitcommit: ef8d6b71fbd962fb3f7081b21724e67a91111a92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/01/2021
ms.locfileid: "60077240"
---
# <a name="deploying-microsoft-365-apps-for-shared-use-on-rds-terminal-server-or-vdi"></a>部署Microsoft 365 应用版在 RDS、终端服务器或 VDI 上共享使用

若要使用Microsoft 365 应用版远程桌面服务 (RDS) ，以前是终端服务，您必须：

- 如果您运行的是较旧版本的 Windows (例如 Windows 7 SP1、Windows Server 2008 R2) ，请使用简单修补程序将 TLS 1.2 启用为默认值。 有关简单的修复和详细信息，请参阅 Update [to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/en-us/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392#bkmk_easy)。 
- 具有包含以前Microsoft 365 企业应用版 (Plus Office 365) 的计划。 例如，Office 365 E3 Microsoft 365 E5或包括桌面版 Project 或 Visio 的任何计划（如 Project 计划 3 或 Visio 计划 2）或 Microsoft 365 商业高级版 计划（其中还包括Microsoft 365 商业应用版。
- 启用共享计算机激活。 有关详细信息，请参阅[Overview of shared computer activation for Microsoft 365 应用版](https://docs.microsoft.com/deployoffice/overview-shared-computer-activation)。

**注意**：若要Microsoft 365 应用版计算机激活模式安装，请下载并运行 [Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal)支持和恢复助手。 有关使用 Office 部署工具自定义安装的先决条件、设置说明和指南的详细信息，请参阅 Deploy [Microsoft 365 应用版 by using Remote Desktop Services](https://docs.microsoft.com/deployoffice/deploy-microsoft-365-apps-remote-desktop-services)。

若要修复与共享计算机激活相关的错误，请参阅：

- [排查用户共享计算机激活Microsoft 365 应用版](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation)
- [重置 Microsoft 365 企业版应用激活状态](https://docs.microsoft.com/office/troubleshoot/activation/reset-office-365-proplus-activation-state)

如果要从 RDS Microsoft 365 应用版 RDS Microsoft 365 管理中心使用默认安装设置，请按照以下步骤操作：

1. 检查Microsoft 365计划。 有关详细信息，请参阅我[拥有哪些订阅？。](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

1. 如有必要，切换到其他Microsoft 365计划。 有关详细信息，请参阅 [升级到其他计划](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan)。

1. 如果Microsoft 365 应用版已使用任何其他不兼容计划安装在 RDS 服务器上，请通过"控制面板""  >  **卸载程序"将其卸载**。 如果遇到问题，请通过下载 Microsoft 支持和恢复助手[卸载](https://aka.ms/SARA-OfficeUninstall-Alchemy)。

1. 在 RDS 服务器上，使用管理员帐户Microsoft 365 管理中心登录服务器，然后[安装Office。](https://portal.office.com/OLS/MySoftware.aspx)

   安装Office后，请不要打开或登录到任何 Office 应用程序。

1. 在 RDS 服务器上，通过编辑注册表启用共享计算机激活：

   1. 右键单击Windows左下角的"运行"按钮，然后选择"**运行"。** 在"打开"框中，键入 **regedit**，然后选择"确定 **"。**

   1. 当系统提示允许注册表编辑器对设备进行更改时，请选择"**是"。**

   1. 在注册表编辑器的 HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration 下，添加一个设置为 **1** 的 **SharedComputerLicensing** 字符串值。

1. 在 RDS 服务器上，以最终用户身份登录并验证共享计算机激活是否Microsoft 365 应用版。 

   有关详细信息，请参阅[验证共享计算机激活是否已启用Microsoft 365 应用版。](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation#verify-that-shared-computer-activation-is-enabled-for-microsoft-365-apps)