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
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="12b78-102">在 RDS、终端服务器或 VDI 上部署 Office 365 专业增强版以供共享使用</span><span class="sxs-lookup"><span data-stu-id="12b78-102">Deploying Office 365 ProPlus for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="12b78-103">若要使用远程桌面服务（RDS）（以前称为 "终端服务"）部署 Office 365 专业增强版，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="12b78-103">To deploy Office 365 ProPlus using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
- <span data-ttu-id="12b78-104">您必须拥有 Microsoft 365 For Business plan 或包含 Office 365 专业增强版的 Office 365 计划（如 Office 365 企业版 E3 或企业版 E5）。</span><span class="sxs-lookup"><span data-stu-id="12b78-104">You must have a Microsoft 365 For Business plan or an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span>
   > [!NOTE] 
   > <span data-ttu-id="12b78-105">Office 365 商业版和 Office 365 商业高级版计划不包括 Office 365 专业增强版。</span><span class="sxs-lookup"><span data-stu-id="12b78-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>
- <span data-ttu-id="12b78-106">您必须启用[共享计算机激活](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)。</span><span class="sxs-lookup"><span data-stu-id="12b78-106">You must enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

> [!NOTE]
> <span data-ttu-id="12b78-107">您还可以下载并运行[Microsoft 支持和恢复助理](https://aka.ms/SaRA_OfficeSCA_M365Portal)，以在共享计算机激活模式下安装 Office 365 专业增强版。</span><span class="sxs-lookup"><span data-stu-id="12b78-107">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Office 365 ProPlus in shared computer activation mode.</span></span>

<span data-ttu-id="12b78-108">有关使用 Office 部署工具的自定义安装的先决条件、安装程序说明和指南的详细信息，请参阅[Deploy Office 365 专业增强版 by Using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)。</span><span class="sxs-lookup"><span data-stu-id="12b78-108">For more information on prerequisites, setup instructions, and guidance on customized installations by using the Office Deployment Tool, see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>

<span data-ttu-id="12b78-109">修复与共享计算机激活相关的错误：</span><span class="sxs-lookup"><span data-stu-id="12b78-109">To fix errors related to shared computer activation:</span></span>
- <span data-ttu-id="12b78-110">请参阅[使用 Office 365 专业增强版的共享计算机激活解决问题](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)。</span><span class="sxs-lookup"><span data-stu-id="12b78-110">See [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
- <span data-ttu-id="12b78-111">请参阅[重置 Office 365 专业增强版激活状态](https://go.microsoft.com/fwlink/?linkid=2109218)。</span><span class="sxs-lookup"><span data-stu-id="12b78-111">See [Reset Office 365 ProPlus activation state](https://go.microsoft.com/fwlink/?linkid=2109218).</span></span>

<span data-ttu-id="12b78-112">如果要从 Microsoft 365 管理中心（***使用默认安装设置***）在 RDS 上安装 Office 365 专业增强版，请执行以下步骤：</span><span class="sxs-lookup"><span data-stu-id="12b78-112">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps:</span></span>

1.  <span data-ttu-id="12b78-113">检查您拥有的 Office 365 计划。</span><span class="sxs-lookup"><span data-stu-id="12b78-113">Check what Office 365 plan you have.</span></span> <span data-ttu-id="12b78-114">[了解如何](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)操作。</span><span class="sxs-lookup"><span data-stu-id="12b78-114">[Learn how](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).</span></span>
2.  <span data-ttu-id="12b78-115">如有必要，请切换到不同的 Office 365 计划。</span><span class="sxs-lookup"><span data-stu-id="12b78-115">If necessary, switch to a different Office 365 plan.</span></span> <span data-ttu-id="12b78-116">[了解如何](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)操作。</span><span class="sxs-lookup"><span data-stu-id="12b78-116">[Learn how](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).</span></span>
3.  <span data-ttu-id="12b78-117">如果已使用任何其他 Office 365 计划在 RDS 服务器上安装了 Office，请将其卸载。</span><span class="sxs-lookup"><span data-stu-id="12b78-117">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="12b78-118">例如，转到 **"控制面板"** > **卸载程序**。</span><span class="sxs-lookup"><span data-stu-id="12b78-118">For example, by going to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="12b78-119">如果遇到问题，请使用[Microsoft 支持和恢复助手](https://aka.ms/SARA-OfficeUninstall-Alchemy)卸载。</span><span class="sxs-lookup"><span data-stu-id="12b78-119">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>
4.  <span data-ttu-id="12b78-120">在 RDS 服务器上，使用管理员帐户登录 Microsoft 365 管理中心并[安装 Office 365 专业增强版](https://portal.office.com/OLS/MySoftware.aspx)。</span><span class="sxs-lookup"><span data-stu-id="12b78-120">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
5.  <span data-ttu-id="12b78-121">安装 Office 后，请***不要打开或登录***任何 Office 应用程序。</span><span class="sxs-lookup"><span data-stu-id="12b78-121">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>
6.  <span data-ttu-id="12b78-122">在 RDS 服务器上，通过执行以下步骤，通过编辑注册表来启用共享计算机激活：</span><span class="sxs-lookup"><span data-stu-id="12b78-122">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
   1. <span data-ttu-id="12b78-123">右键单击屏幕左下角的 "Windows" 按钮，然后选择 "**运行**"。</span><span class="sxs-lookup"><span data-stu-id="12b78-123">Right-click the Windows button in the lower left-corner of your screen and select **Run**.</span></span> <span data-ttu-id="12b78-124">在 "打开" 框中，键入 " **regedit**"，然后选择 **"确定"**。</span><span class="sxs-lookup"><span data-stu-id="12b78-124">In the Open box, type **regedit**, and then select **OK**.</span></span>
   2. <span data-ttu-id="12b78-125">当系统提示允许注册表编辑器对设备进行更改时，选择 **"是"** 。</span><span class="sxs-lookup"><span data-stu-id="12b78-125">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
   3. <span data-ttu-id="12b78-126">在注册表编辑器中，在 HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration. 下添加**SharedComputerLicensing**的字符串值设置为1。</span><span class="sxs-lookup"><span data-stu-id="12b78-126">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>
   4. <span data-ttu-id="12b78-127">在 RDS 服务器上，***以最终用户的形式登录***，并[验证是否已为 Office 365 专业增强版启用了共享计算机激活](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded)。</span><span class="sxs-lookup"><span data-stu-id="12b78-127">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

