---
title: 在 RDS、终端服务器或 VDI 上部署 Office 365 专业增强版以供共享使用
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 12/9/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 2312cca9ebf5dad1322bc98335cef6a6bc81f03e
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959450"
---
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a>在 RDS、终端服务器或 VDI 上部署 Office 365 专业增强版以供共享使用

若要使用远程桌面服务（RDS）（以前称为 "终端服务"）部署 Office 365 专业增强版，请执行以下操作：
- 您必须拥有 Microsoft 365 For Business plan 或包含 Office 365 专业增强版的 Office 365 计划（如 Office 365 企业版 E3 或企业版 E5）。
   > [!NOTE] 
   > Office 365 商业版和 Office 365 商业高级版计划不包括 Office 365 专业增强版。
- 您必须启用[共享计算机激活](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)。

> [!NOTE]
> 您还可以下载并运行[Microsoft 支持和恢复助理](https://aka.ms/SaRA_OfficeSCA_M365Portal)，以在共享计算机激活模式下安装 Office 365 专业增强版。

有关使用 Office 部署工具的自定义安装的先决条件、安装程序说明和指南的详细信息，请参阅[Deploy Office 365 专业增强版 by Using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)。

修复与共享计算机激活相关的错误：
- 请参阅[使用 Office 365 专业增强版的共享计算机激活解决问题](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)。
- 请参阅[重置 Office 365 专业增强版激活状态](https://go.microsoft.com/fwlink/?linkid=2109218)。

如果要从 Microsoft 365 管理中心（***使用默认安装设置***）在 RDS 上安装 Office 365 专业增强版，请执行以下步骤：

1.  检查您拥有的 Office 365 计划。 [了解如何](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)操作。
2.  如有必要，请切换到不同的 Office 365 计划。 [了解如何](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)操作。
3.  如果已使用任何其他 Office 365 计划在 RDS 服务器上安装了 Office，请将其卸载。 例如，转到 **"控制面板"** > **卸载程序**。 如果遇到问题，请使用[Microsoft 支持和恢复助手](https://aka.ms/SARA-OfficeUninstall-Alchemy)卸载。
4.  在 RDS 服务器上，使用管理员帐户登录 Microsoft 365 管理中心并[安装 Office 365 专业增强版](https://portal.office.com/OLS/MySoftware.aspx)。
5.  安装 Office 后，请***不要打开或登录***任何 Office 应用程序。
6.  在 RDS 服务器上，通过执行以下步骤，通过编辑注册表来启用共享计算机激活：
   1. 右键单击屏幕左下角的 "Windows" 按钮，然后选择 "**运行**"。 在 "打开" 框中，键入 " **regedit**"，然后选择 **"确定"**。
   2. 当系统提示允许注册表编辑器对设备进行更改时，选择 **"是"** 。
   3. 在注册表编辑器中，在 HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration. 下添加**SharedComputerLicensing**的字符串值设置为1。
   4. 在 RDS 服务器上，***以最终用户的形式登录***，并[验证是否已为 Office 365 专业增强版启用了共享计算机激活](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded)。

