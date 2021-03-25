---
title: 部署 Microsoft 365 企业应用版以在 RDS、终端服务器或 VDI 上共享使用
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
ms.openlocfilehash: a57be7fcf9d8236a51dc4b38e33ad1c2ac717f11
ms.sourcegitcommit: 2eab0980268e08a58014459d44a08a1cc34a17d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200663"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>部署 Microsoft 365 企业应用版以在 RDS、终端服务器或 VDI 上共享使用

若要使用远程桌面服务部署 Microsoft 365 企业应用版， (RDS) 以前称为终端服务：

- 必须具有 Microsoft 365 商业版计划或包含 Microsoft 365 企业应用版（如 Office 365 企业版 E3 或企业版 E5）的 Office 365 计划。
   > [!NOTE]
   > Microsoft 365 商业应用版和 Microsoft 365 商业标准版计划不包括 Microsoft 365 企业应用版。
- 必须启用 [共享计算机激活](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)。

> [!NOTE]
> 还可以下载并运行 Microsoft [支持和恢复助手](https://aka.ms/SaRA_OfficeSCA_M365Portal) ，以在共享计算机激活模式下安装 Microsoft 365 企业应用版。

有关使用 Office 部署工具的自定义安装的先决条件、设置说明和指南详细信息，请参阅使用远程桌面服务部署 [Microsoft 365](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)企业应用版。

若要修复与共享计算机激活相关的错误，

- 请参阅 [排查 Microsoft 365](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)企业应用版共享计算机激活问题。
- 参见[重置 Microsoft 365 企业版应用激活状态](https://go.microsoft.com/fwlink/?linkid=2109218)。

如果要从使用默认安装设置的 Microsoft 365 管理中心在 RDS 上安装 Microsoft 365 企业应用版，请使用以下步骤：

1. 检查你拥有哪些订阅。 [了解如何。](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)
2. 如有必要，切换到其他订阅。 [了解如何。](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)
3. 如果 RDS 服务器上已经使用任何其他 Microsoft 订阅安装了 Office，请卸载它。 例如，通过进入控制面板 **卸载**  >  **程序**。 如果正在运行 [问题，](https://aka.ms/SARA-OfficeUninstall-Alchemy) 使用 Microsoft 支持和恢复助手卸载。
4. 在 RDS 服务器上，使用管理员帐户登录到 Microsoft 365 管理中心，然后安装 [Microsoft 365 企业应用版](https://portal.office.com/OLS/MySoftware.aspx)。
5. 安装 Office 后 ***，不要打开或登录任何*** Office 应用程序。
6. 在 RDS 服务器上，通过按照以下步骤编辑注册表来启用共享计算机激活：
   1. 右键单击屏幕左下角的 Windows 按钮， **然后选择运行**。 在"打开"框中，键入 **regedit**，然后选择"确定 **"。**
   2. 当 **系统** 提示允许注册表编辑器对设备进行更改时，选择"是"。
   3. 在注册表编辑器中，将 **SharedComputerLicensing** 的字符串值添加到 HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration 下，将设置为 1。
   4. 在 RDS 服务器上 ***，以*** 最终用户身份登录并验证共享计算机激活是否已启用 [Microsoft 365 企业应用版](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)。
