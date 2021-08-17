---
title: 在终端服务器上安装办公室 - 未授权
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 7e435df1515878ab4fe935ab8148daee29b8e3820095fc6e49db45de4c6279db
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54055148"
---
# <a name="installing-office-on-a-terminal-server"></a>在Office服务器上安装客户端

使用 RDS Microsoft 365 企业应用版 RDS Windows (远程桌面服务) 远程桌面服务) 远程桌面服务部署客户端：
  
- 你必须拥有包含 Microsoft 365 订阅，Microsoft 365 企业应用版 E3 或 Office 365 企业版 E5 Enterprise订阅。 Microsoft 365 商业应用版和Microsoft 365 商业应用版 高级版计划不包括Microsoft 365 企业应用版。

- 需要启用共享 [计算机激活](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)。

如果要从 RDS Microsoft 365 企业应用版使用默认安装设置的 RDS Microsoft 365 管理中心，请使用以下步骤。

> [!TIP]
> 还可以下载并运行 Microsoft[支持和恢复助手](https://aka.ms/SaRA_OfficeSCA_M365Portal)以Microsoft 365 企业应用版计算机激活模式进行安装。
  
1. 检查Microsoft 365订阅。 [了解操作方式](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. 如有必要，切换到其他Microsoft 365订阅。 [了解操作方式](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. 如果Office已使用任何其他订阅安装在 RDS 服务器上，Microsoft 365卸载它。 例如，通过进入"控制面板 \> ""卸载程序"。 如果支持和恢复助手[问题](https://aka.ms/SARA-OfficeUninstall-Alchemy)，使用 Microsoft 支持和恢复助手卸载。

4. 在 RDS 服务器上，使用管理员帐户Microsoft 365 管理中心登录服务器，然后[安装Microsoft 365 企业应用版。](https://portal.office.com/OLS/MySoftware.aspx)

5. 安装Office后，请不要打开或 ***登录到*** 任何 Office 应用程序。

6. 在 RDS 服务器上，通过按照以下步骤编辑注册表来启用共享计算机激活：

1. 右键单击Windows左下角的"运行"按钮，然后选择"运行"。 在"打开"框中，键入 **regedit**，然后选择"确定"。

2. 当系统提示允许注册表编辑器对设备进行更改时，选择"是"。

3. 在注册表编辑器中，将 **SharedComputerLicensing** 的字符串值添加到 HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration 下，将设置为 1。

7. 在 RDS 服务器上 ***，以*** 最终用户身份登录并验证共享计算机激活是否已启用 [Microsoft 365 企业应用版。](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)

有关使用 Office 部署工具的自定义安装的先决条件、设置说明和指南的更多详细信息，请参阅使用远程桌面服务部署[Microsoft 365 企业应用版。](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)
  
若要修复与共享计算机激活相关的错误，请参阅[Troubleshoot issues with shared computer activation for Microsoft 365 企业应用版](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)。
  