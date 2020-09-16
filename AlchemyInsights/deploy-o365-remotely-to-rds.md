---
title: 在 RDS、终端服务器或 VDI 上部署适用于企业的 Microsoft 365 应用程序以供共享使用
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 22ded616e82b2e82023b55a1d3ca6251cfb71712
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745525"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>在 RDS、终端服务器或 VDI 上部署适用于企业的 Microsoft 365 应用程序以供共享使用

若要使用远程桌面服务部署适用于企业的 Microsoft 365 应用程序 (RDS) （以前称为 "终端服务"）：
- 您必须拥有 Microsoft 365 For Business plan 或 Office 365 计划，其中包含适用于企业的 Microsoft 365 应用程序，例如 Office 365 企业版 E3 或企业版 E5。
   > [!NOTE] 
   > 适用于商业和 Microsoft 365 商业高级标准计划的 Microsoft 365 应用程序不包含适用于企业的 Microsoft 365 应用程序。
- 您必须启用 [共享计算机激活](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)。

> [!NOTE]
> 您还可以下载并运行 [Microsoft 支持和恢复助理](https://aka.ms/SaRA_OfficeSCA_M365Portal) ，以在共享计算机激活模式下安装适用于企业的 Microsoft 365 应用程序。

有关使用 Office 部署工具的自定义安装的先决条件、安装程序说明和指南的详细信息，请参阅 [使用远程桌面服务部署适用于企业的 Microsoft 365 应用程序](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)。

修复与共享计算机激活相关的错误：
- 请参阅 [疑难解答 Microsoft 365 Apps for enterprise 中的共享计算机激活的问题](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)。
- 参见[重置 Microsoft 365 企业版应用激活状态](https://go.microsoft.com/fwlink/?linkid=2109218)。

如果要从 Microsoft 365 管理中心（ ***使用默认安装设置***）在 RDS 上安装 Microsoft 365 应用程序，请执行以下步骤：

1.    检查您拥有的订阅。 [了解如何](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)操作。
2.    如有必要，请切换到其他订阅。 [了解如何](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)操作。
3.    如果已使用任何其他 Microsoft 订阅在 RDS 服务器上安装了 Office，请将其卸载。 例如，转到 **"控制面板"**  >  **卸载程序**。 如果遇到问题，请使用 [Microsoft 支持和恢复助手](https://aka.ms/SARA-OfficeUninstall-Alchemy) 卸载。
4.    在 RDS 服务器上，使用管理员帐户登录 Microsoft 365 管理中心并 [安装适用于企业的 microsoft 365 应用程序](https://portal.office.com/OLS/MySoftware.aspx)。
5.    安装 Office 后，请 ***不要打开或登录*** 任何 Office 应用程序。
6.    在 RDS 服务器上，通过执行以下步骤，通过编辑注册表来启用共享计算机激活：
   1. 右键单击屏幕左下角的 "Windows" 按钮，然后选择 " **运行**"。 在 "打开" 框中，键入 " **regedit**"，然后选择 **"确定"**。
   2. 当系统提示允许注册表编辑器对设备进行更改时，选择 **"是"** 。
   3. 在注册表编辑器中，在 HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration. 下添加 **SharedComputerLicensing** 的字符串值设置为1。
   4. 在 RDS 服务器上， ***以最终用户的形式登录*** ，并 [验证是否已为 Microsoft 365 的企业版应用程序激活共享计算机激活](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)。

