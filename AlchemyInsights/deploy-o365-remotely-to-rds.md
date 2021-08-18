---
title: 部署Microsoft 365 企业应用版在 RDS、终端服务器或 VDI 上共享使用
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
ms.openlocfilehash: b8df97c19937a757c1de9865b6c7b8d1cddfd62d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325593"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>部署Microsoft 365 企业应用版在 RDS、终端服务器或 VDI 上共享使用

若要使用Microsoft 365 企业应用版远程桌面服务 (RDS) ，以前称为终端服务：

- 必须拥有包含 Microsoft 365 For Business 计划或 Office 365 计划Microsoft 365 企业应用版 E3 或 Office 365 企业版 E5 Enterprise计划。
   **注意**：Microsoft 365 商业应用版和Microsoft 365 商业标准版计划不包括Microsoft 365 企业应用版。
- 必须启用 [共享计算机激活](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)。

**注意**：还可以下载并运行 Microsoft [支持和恢复助手](https://aka.ms/SaRA_OfficeSCA_M365Portal)以Microsoft 365 企业应用版计算机激活模式进行安装。

有关使用 Office 部署工具进行自定义安装的先决条件、设置说明和指南，请参阅使用远程桌面服务部署[Microsoft 365 企业应用版。](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)

若要修复与共享计算机激活相关的错误，

- 请参阅[Troubleshoot issues with shared computer activation for Microsoft 365 企业应用版](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)。
- 参见[重置 Microsoft 365 企业版应用激活状态](https://go.microsoft.com/fwlink/?linkid=2109218)。

如果要从 RDS Microsoft 365 企业应用版使用默认安装设置的 RDS Microsoft 365 管理中心，请执行以下步骤：

1. 检查你拥有哪些订阅。 [了解如何。](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)
2. 如有必要，切换到其他订阅。 [了解如何。](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)
3. 如果Office任何其他 Microsoft 订阅已在 RDS 服务器上安装，请将其卸载。 例如，通过进入"**控制面板**  >  **""卸载程序"。** 如果支持和恢复助手[问题](https://aka.ms/SARA-OfficeUninstall-Alchemy)，请卸载 Microsoft 支持和恢复助手。
4. 在 RDS 服务器上，使用管理员帐户Microsoft 365 管理中心登录服务器，然后[安装Microsoft 365 企业应用版。](https://portal.office.com/OLS/MySoftware.aspx)
5. 安装Office后，请不要打开或 ***登录到*** 任何 Office 应用程序。
6. 在 RDS 服务器上，通过按照以下步骤编辑注册表来启用共享计算机激活：
   1. 右键单击Windows左下角的"运行"按钮，然后选择"**运行"。** 在"打开"框中，键入 **regedit**，然后选择"确定 **"。**
   2. 当 **系统** 提示允许注册表编辑器对设备进行更改时，选择"是"。
   3. 在注册表编辑器中，将 **SharedComputerLicensing** 的字符串值添加到 HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration 下，将设置为 1。
   4. 在 RDS 服务器上 ***，以*** 最终用户身份登录，并验证共享计算机激活是否 [Microsoft 365 企业应用版。](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)
