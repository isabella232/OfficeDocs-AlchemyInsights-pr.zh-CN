---
title: 在终端服务器-未经授权上安装 office
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 73d5128b55cae7712c48be9e2d05e558c3ba2e5c
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29459499"
---
# <a name="installing-office-on-a-terminal-server"></a>在终端服务器上安装 Office

部署 Office 365 ProPlus 使用远程桌面服务 (RDS) 的 Windows 服务器上，以前称为终端服务：
  
- 您必须具有包含 Office 365 ProPlus，例如 Office 365 企业版 E3 或企业 E5 的 Office 365 计划。Office 365 企业版和 Office 365 企业高级版规划中不包括 Office 365 ProPlus。
    
- 您需要启用[共享的计算机激活](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)。
    
如果您想要安装 Office 365 ProPlus RDS 上从 Office 365 门户，* **其使用默认安装设置** *，请按照下列步骤： 
  
1. 检查您有哪些 Office 365 计划。[了解如何](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)
    
2. 如果需要，切换到不同的 Office 365 计划。[了解如何](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)
    
3. 如果已使用任何其他 Office 365 计划的 RDS 服务器上安装 Office，则先卸载它。例如，通过转到 Control Panel\>卸载程序。卸载使用[Microsoft 支持和恢复助手](https://aka.ms/SARA-OfficeUninstall-Alchemy)，如果您运行到问题。 
    
4. 在 RDS 服务器上，登录到您的管理员帐户和[安装 Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx)的 Office 365 门户。
    
5. 安装 Office 后，* **不要打开或登录** * 任何 Office 应用程序。 
    
6. 在 RDS 服务器上，通过编辑注册表，按照以下步骤来启用共享的计算机激活：
    
1. 右键单击屏幕的左上角的 Windows 按钮，然后选择运行。在打开框中，键入**regedit**，，然后选择确定。 
    
2. 选择是时提示您允许注册表编辑器来更改您的设备。
    
3. 在注册表编辑器中，设置为 1 HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration 下添加**SharedComputerLicensing**字符串值。 
    
7. 在 RDS 服务器上，* **登录为最终用户** *，并[验证是否已为 Office 365 ProPlus 启用共享的计算机激活](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded)。
    
有关先决条件、 安装说明和使用 Office 部署工具自定义安装指南的详细信息，请参阅[部署 Office 365 ProPlus 使用远程桌面服务](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)。
  
若要解决与共享的计算机激活相关的错误，请参阅[Troubleshoot 共享的计算机激活 Office 365 ProPlus 的问题](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)。
  

