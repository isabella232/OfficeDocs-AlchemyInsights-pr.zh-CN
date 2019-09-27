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
ms.openlocfilehash: 51d1a66fdf9774bbe58bfdbe89317bc93834be09
ms.sourcegitcommit: 5e6a805fb0b41d714ca1cf90e23b8e2daa90f90e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37205399"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="aab07-102">在终端服务器上安装 Office</span><span class="sxs-lookup"><span data-stu-id="aab07-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="aab07-103">使用远程桌面服务（RDS）（以前称为 "终端服务"）在 Windows 服务器上部署 Office 365 专业增强版时，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="aab07-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="aab07-104">您必须拥有包含 Office 365 专业增强版的 Office 365 计划，如 Office 365 企业版 E3 或企业版 E5。</span><span class="sxs-lookup"><span data-stu-id="aab07-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="aab07-105">Office 365 商业版和 Office 365 商业高级版计划不包括 Office 365 专业增强版。</span><span class="sxs-lookup"><span data-stu-id="aab07-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>

- <span data-ttu-id="aab07-106">您需要启用[共享计算机激活](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)。</span><span class="sxs-lookup"><span data-stu-id="aab07-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="aab07-107">如果要从 Microsoft 365 管理中心（***使用默认安装设置***）在 RDS 上安装 Office 365 专业增强版，请执行以下步骤。</span><span class="sxs-lookup"><span data-stu-id="aab07-107">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="aab07-108">您还可以下载并运行[Microsoft 支持和恢复助理](https://aka.ms/SaRA_OfficeSCA_M365Portal)，以在共享计算机激活模式下安装 Office 365 专业增强版。</span><span class="sxs-lookup"><span data-stu-id="aab07-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Office 365 ProPlus in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="aab07-109">检查您拥有的 Office 365 计划。</span><span class="sxs-lookup"><span data-stu-id="aab07-109">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="aab07-110">了解方法</span><span class="sxs-lookup"><span data-stu-id="aab07-110">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="aab07-111">如有必要，请切换到不同的 Office 365 计划。</span><span class="sxs-lookup"><span data-stu-id="aab07-111">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="aab07-112">了解方法</span><span class="sxs-lookup"><span data-stu-id="aab07-112">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="aab07-113">如果已使用任何其他 Office 365 计划在 RDS 服务器上安装了 Office，请将其卸载。</span><span class="sxs-lookup"><span data-stu-id="aab07-113">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="aab07-114">例如，转到 "控制面板" \>卸载程序。</span><span class="sxs-lookup"><span data-stu-id="aab07-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="aab07-115">如果遇到问题，请使用[Microsoft 支持和恢复助手](https://aka.ms/SARA-OfficeUninstall-Alchemy)卸载。</span><span class="sxs-lookup"><span data-stu-id="aab07-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="aab07-116">在 RDS 服务器上，使用管理员帐户登录 Microsoft 365 管理中心并[安装 Office 365 专业增强版](https://portal.office.com/OLS/MySoftware.aspx)。</span><span class="sxs-lookup"><span data-stu-id="aab07-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="aab07-117">安装 Office 后，请***不要打开或登录***任何 Office 应用程序。</span><span class="sxs-lookup"><span data-stu-id="aab07-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="aab07-118">在 RDS 服务器上，通过执行以下步骤，通过编辑注册表来启用共享计算机激活：</span><span class="sxs-lookup"><span data-stu-id="aab07-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="aab07-119">右键单击屏幕左下角的 "Windows" 按钮，然后选择 "运行"。</span><span class="sxs-lookup"><span data-stu-id="aab07-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="aab07-120">在 "打开" 框中，键入 " **regedit**"，然后选择 "确定"。</span><span class="sxs-lookup"><span data-stu-id="aab07-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="aab07-121">当系统提示允许注册表编辑器对设备进行更改时，选择 "是"。</span><span class="sxs-lookup"><span data-stu-id="aab07-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="aab07-122">在注册表编辑器中，在 HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration. 下添加一个**SharedComputerLicensing**设置为1的字符串值。</span><span class="sxs-lookup"><span data-stu-id="aab07-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="aab07-123">在 RDS 服务器上，***以最终用户的形式登录***，并[验证是否已为 Office 365 专业增强版启用了共享计算机激活](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded)。</span><span class="sxs-lookup"><span data-stu-id="aab07-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="aab07-124">有关使用 Office 部署工具的自定义安装的先决条件、设置说明和指南的详细信息，请参阅[Deploy Office 365 专业增强版 by Using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)。</span><span class="sxs-lookup"><span data-stu-id="aab07-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="aab07-125">若要修复与共享计算机激活相关的错误，请参阅[针对 Office 365 专业增强版的共享计算机激活解决问题](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)。</span><span class="sxs-lookup"><span data-stu-id="aab07-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  