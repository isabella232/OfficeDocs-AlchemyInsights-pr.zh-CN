---
title: 在终端服务器上安装 office-未授权
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 6e952513679c9ac66f8de2b43d6d243cf17ff789
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010604"
---
# <a name="installing-office-on-a-terminal-server"></a>在终端服务器上安装 Office

使用远程桌面服务（RDS）（以前称为 "终端服务"）在 Windows 服务器上部署适用于企业的 Microsoft 365 应用：
  
- 您必须拥有包含适用于企业的 Microsoft 365 应用程序的 Microsoft 365 订阅，例如 Office 365 企业版 E3 或企业版 E5。 适用于商业的 Microsoft 365 apps 和 Microsoft 365 应用程序高级计划不包含适用于企业的 Microsoft 365 应用程序。

- 您需要启用[共享计算机激活](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)。

如果要从 Microsoft 365 管理中心（***使用默认安装设置***）在 RDS 上安装 Microsoft 365 应用程序，请执行以下步骤。

> [!TIP]
> 您还可以下载并运行[Microsoft 支持和恢复助理](https://aka.ms/SaRA_OfficeSCA_M365Portal)，以在共享计算机激活模式下安装适用于企业的 Microsoft 365 应用程序。
  
1. 检查您拥有的 Microsoft 365 订阅。 [了解方法](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. 如有必要，请切换到其他 Microsoft 365 订阅。 [了解方法](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. 如果已使用任何其他 Microsoft 365 订阅在 RDS 服务器上安装了 Office，请将其卸载。 例如，转到 "控制面板" \>卸载程序。 如果遇到问题，请使用[Microsoft 支持和恢复助手](https://aka.ms/SARA-OfficeUninstall-Alchemy)卸载。

4. 在 RDS 服务器上，使用管理员帐户登录 Microsoft 365 管理中心并[安装适用于企业的 microsoft 365 应用程序](https://portal.office.com/OLS/MySoftware.aspx)。

5. 安装 Office 后，请***不要打开或登录***任何 Office 应用程序。

6. 在 RDS 服务器上，通过执行以下步骤，通过编辑注册表来启用共享计算机激活：

1. 右键单击屏幕左下角的 "Windows" 按钮，然后选择 "运行"。 在 "打开" 框中，键入 " **regedit**"，然后选择 "确定"。

2. 当系统提示允许注册表编辑器对设备进行更改时，选择 "是"。

3. 在注册表编辑器中，在 HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration. 下添加**SharedComputerLicensing**的字符串值设置为1。

7. 在 RDS 服务器上，***以最终用户的形式登录***，并[验证是否已为 Microsoft 365 的企业版应用程序激活共享计算机激活](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)。

有关使用 Office 部署工具的自定义安装的先决条件、设置说明和指南的详细信息，请参阅[Deploy Microsoft 365 Apps for enterprise by Using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)。
  
若要修复与共享计算机激活相关的错误，请参阅[针对企业共享计算机激活的 Microsoft 365 应用程序的故障排除问题](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)。
  