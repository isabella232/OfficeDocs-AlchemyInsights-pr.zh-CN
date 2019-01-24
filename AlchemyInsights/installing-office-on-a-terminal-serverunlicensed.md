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
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="f3bd7-102">在终端服务器上安装 Office</span><span class="sxs-lookup"><span data-stu-id="f3bd7-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="f3bd7-103">部署 Office 365 ProPlus 使用远程桌面服务 (RDS) 的 Windows 服务器上，以前称为终端服务：</span><span class="sxs-lookup"><span data-stu-id="f3bd7-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="f3bd7-p101">您必须具有包含 Office 365 ProPlus，例如 Office 365 企业版 E3 或企业 E5 的 Office 365 计划。Office 365 企业版和 Office 365 企业高级版规划中不包括 Office 365 ProPlus。</span><span class="sxs-lookup"><span data-stu-id="f3bd7-p101">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5. The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>
    
- <span data-ttu-id="f3bd7-106">您需要启用[共享的计算机激活](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)。</span><span class="sxs-lookup"><span data-stu-id="f3bd7-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>
    
<span data-ttu-id="f3bd7-107">如果您想要安装 Office 365 ProPlus RDS 上从 Office 365 门户，\* **其使用默认安装设置** \*，请按照下列步骤：</span><span class="sxs-lookup"><span data-stu-id="f3bd7-107">If you want to install Office 365 ProPlus on RDS from the Office 365 portal, \*\* *which uses default installation settings* \*\*, follow these steps:</span></span> 
  
1. <span data-ttu-id="f3bd7-p102">检查您有哪些 Office 365 计划。[了解如何](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)</span><span class="sxs-lookup"><span data-stu-id="f3bd7-p102">Check what Office 365 plan you have. [Learn how](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)</span></span>
    
2. <span data-ttu-id="f3bd7-p103">如果需要，切换到不同的 Office 365 计划。[了解如何](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)</span><span class="sxs-lookup"><span data-stu-id="f3bd7-p103">If necessary, switch to a different Office 365 plan. [Learn how](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)</span></span>
    
3. <span data-ttu-id="f3bd7-p104">如果已使用任何其他 Office 365 计划的 RDS 服务器上安装 Office，则先卸载它。例如，通过转到 Control Panel\>卸载程序。卸载使用[Microsoft 支持和恢复助手](https://aka.ms/SARA-OfficeUninstall-Alchemy)，如果您运行到问题。</span><span class="sxs-lookup"><span data-stu-id="f3bd7-p104">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it. For example, by going to Control Panel \> Uninstall a program. Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span> 
    
4. <span data-ttu-id="f3bd7-115">在 RDS 服务器上，登录到您的管理员帐户和[安装 Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx)的 Office 365 门户。</span><span class="sxs-lookup"><span data-stu-id="f3bd7-115">On the RDS server, sign in to the Office 365 portal with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
    
5. <span data-ttu-id="f3bd7-116">安装 Office 后，\* **不要打开或登录** \* 任何 Office 应用程序。</span><span class="sxs-lookup"><span data-stu-id="f3bd7-116">After Office is installed, \*\* *don't open or sign in* \*\* to any Office applications.</span></span> 
    
6. <span data-ttu-id="f3bd7-117">在 RDS 服务器上，通过编辑注册表，按照以下步骤来启用共享的计算机激活：</span><span class="sxs-lookup"><span data-stu-id="f3bd7-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
    
1. <span data-ttu-id="f3bd7-p105">右键单击屏幕的左上角的 Windows 按钮，然后选择运行。在打开框中，键入**regedit**，，然后选择确定。</span><span class="sxs-lookup"><span data-stu-id="f3bd7-p105">Right-click the Windows button in the lower left-hand corner of your screen and select Run. In the Open box, type **regedit**, and then select OK.</span></span> 
    
2. <span data-ttu-id="f3bd7-120">选择是时提示您允许注册表编辑器来更改您的设备。</span><span class="sxs-lookup"><span data-stu-id="f3bd7-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>
    
3. <span data-ttu-id="f3bd7-121">在注册表编辑器中，设置为 1 HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration 下添加**SharedComputerLicensing**字符串值。</span><span class="sxs-lookup"><span data-stu-id="f3bd7-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span> 
    
7. <span data-ttu-id="f3bd7-122">在 RDS 服务器上，\* **登录为最终用户** \*，并[验证是否已为 Office 365 ProPlus 启用共享的计算机激活](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded)。</span><span class="sxs-lookup"><span data-stu-id="f3bd7-122">On the RDS server, \*\* *sign in as an end user* \*\* and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>
    
<span data-ttu-id="f3bd7-123">有关先决条件、 安装说明和使用 Office 部署工具自定义安装指南的详细信息，请参阅[部署 Office 365 ProPlus 使用远程桌面服务](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)。</span><span class="sxs-lookup"><span data-stu-id="f3bd7-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="f3bd7-124">若要解决与共享的计算机激活相关的错误，请参阅[Troubleshoot 共享的计算机激活 Office 365 ProPlus 的问题](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)。</span><span class="sxs-lookup"><span data-stu-id="f3bd7-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  

