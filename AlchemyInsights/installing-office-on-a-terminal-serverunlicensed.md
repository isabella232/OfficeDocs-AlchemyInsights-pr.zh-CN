---
title: 在终端服务器上安装 office-未授权
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 971edd9c064b448446ba16361e99df4a2291c14f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2019
ms.locfileid: "32410112"
---
# <a name="installing-office-on-a-terminal-server"></a>在终端服务器上安装 Office

使用远程桌面服务 (RDS) (以前称为 "终端服务") 在 Windows 服务器上部署 Office 365 专业增强版时, 请执行以下操作:
  
- 您必须拥有包含 office 365 专业增强版的 office 365 计划, 如 office 365 企业版 E3 或企业版 E5。 office 365 商业版和 office 365 商业高级版计划不包括 office 365 专业增强版。
    
- 您需要启用[共享计算机激活](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)。
    
如果要从 office 365 门户安装 RDS 上的 office 365 专业增强版, * **使用默认安装设置** *, 请按照以下步骤操作: 
  
1. 检查您拥有的 Office 365 计划。 [了解方法](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)
    
2. 如有必要, 请切换到不同的 Office 365 计划。 [了解方法](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)
    
3. 如果已使用任何其他 office 365 计划在 RDS 服务器上安装了 office, 请将其卸载。 例如, 转到 "控制面板" \>卸载程序。 如果遇到问题, 请使用[Microsoft 支持和恢复助手](https://aka.ms/SARA-OfficeUninstall-Alchemy)卸载。 
    
4. 在 RDS 服务器上, 使用管理员帐户登录到 Office 365 门户, 并[安装 office 365 专业增强版](https://portal.office.com/OLS/MySoftware.aspx)。
    
5. 安装 office 后, * **请勿打开** * 并登录到任何 Office 应用程序。 
    
6. 在 RDS 服务器上, 通过执行以下步骤, 通过编辑注册表来启用共享计算机激活:
    
1. 右键单击屏幕左下角的 "Windows" 按钮, 然后选择 "运行"。 在 "打开" 框中, 键入 " **regedit**", 然后选择 "确定"。 
    
2. 当系统提示允许注册表编辑器对设备进行更改时, 选择 "是"。
    
3. 在注册表编辑器中, 在 HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration. 下添加一个**SharedComputerLicensing**设置为1的字符串值。 
    
7. 在 RDS 服务器上, * * 以*最终用户的形式登录** *, 并[验证是否为 Office 365 专业增强版启用了共享计算机激活](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded)。
    
有关使用 Office 部署工具的自定义安装的先决条件、设置说明和指南的详细信息, 请参阅[Deploy Office 365 专业增强版 by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)。
  
若要修复与共享计算机激活相关的错误, 请参阅[针对 Office 365 专业增强版的共享计算机激活解决问题](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)。
  

