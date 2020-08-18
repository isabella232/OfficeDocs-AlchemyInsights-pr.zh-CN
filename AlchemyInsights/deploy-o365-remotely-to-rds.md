---
title: 在 RDS、终端服务器或 VDI 上部署适用于企业的 Microsoft 365 应用程序以供共享使用
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: bd30d99221e3ddd0b07db0db78009f346babd2d0
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786267"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="05ecd-102">在 RDS、终端服务器或 VDI 上部署适用于企业的 Microsoft 365 应用程序以供共享使用</span><span class="sxs-lookup"><span data-stu-id="05ecd-102">Deploying Microsoft 365 Apps for enterprise for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="05ecd-103">若要使用远程桌面服务部署适用于企业的 Microsoft 365 应用程序 (RDS) （以前称为 "终端服务"）：</span><span class="sxs-lookup"><span data-stu-id="05ecd-103">To deploy Microsoft 365 Apps for enterprise using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
- <span data-ttu-id="05ecd-104">您必须拥有 Microsoft 365 For Business plan 或 Office 365 计划，其中包含适用于企业的 Microsoft 365 应用程序，例如 Office 365 企业版 E3 或企业版 E5。</span><span class="sxs-lookup"><span data-stu-id="05ecd-104">You must have a Microsoft 365 For Business plan or an Office 365 plan that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span>
   > [!NOTE] 
   > <span data-ttu-id="05ecd-105">适用于商业和 Microsoft 365 商业高级标准计划的 Microsoft 365 应用程序不包含适用于企业的 Microsoft 365 应用程序。</span><span class="sxs-lookup"><span data-stu-id="05ecd-105">The Microsoft 365 Apps for business and Microsoft 365 Business Premium Standard plans do not include Microsoft 365 Apps for enterprise.</span></span>
- <span data-ttu-id="05ecd-106">您必须启用 [共享计算机激活](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)。</span><span class="sxs-lookup"><span data-stu-id="05ecd-106">You must enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

> [!NOTE]
> <span data-ttu-id="05ecd-107">您还可以下载并运行 [Microsoft 支持和恢复助理](https://aka.ms/SaRA_OfficeSCA_M365Portal) ，以在共享计算机激活模式下安装适用于企业的 Microsoft 365 应用程序。</span><span class="sxs-lookup"><span data-stu-id="05ecd-107">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>

<span data-ttu-id="05ecd-108">有关使用 Office 部署工具的自定义安装的先决条件、安装程序说明和指南的详细信息，请参阅 [使用远程桌面服务部署适用于企业的 Microsoft 365 应用程序](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)。</span><span class="sxs-lookup"><span data-stu-id="05ecd-108">For more information on prerequisites, setup instructions, and guidance on customized installations by using the Office Deployment Tool, see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>

<span data-ttu-id="05ecd-109">修复与共享计算机激活相关的错误：</span><span class="sxs-lookup"><span data-stu-id="05ecd-109">To fix errors related to shared computer activation:</span></span>
- <span data-ttu-id="05ecd-110">请参阅 [疑难解答 Microsoft 365 Apps for enterprise 中的共享计算机激活的问题](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)。</span><span class="sxs-lookup"><span data-stu-id="05ecd-110">See [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
- <span data-ttu-id="05ecd-111">参见[重置 Microsoft 365 企业版应用激活状态](https://go.microsoft.com/fwlink/?linkid=2109218)。</span><span class="sxs-lookup"><span data-stu-id="05ecd-111">See [Reset Microsoft 365 Apps for enterprise activation state](https://go.microsoft.com/fwlink/?linkid=2109218).</span></span>

<span data-ttu-id="05ecd-112">如果要从 Microsoft 365 管理中心（ ***使用默认安装设置***）在 RDS 上安装 Microsoft 365 应用程序，请执行以下步骤：</span><span class="sxs-lookup"><span data-stu-id="05ecd-112">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps:</span></span>

1.    <span data-ttu-id="05ecd-113">检查您拥有的订阅。</span><span class="sxs-lookup"><span data-stu-id="05ecd-113">Check what subscription you have.</span></span> <span data-ttu-id="05ecd-114">[了解如何](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)操作。</span><span class="sxs-lookup"><span data-stu-id="05ecd-114">[Learn how](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).</span></span>
2.    <span data-ttu-id="05ecd-115">如有必要，请切换到其他订阅。</span><span class="sxs-lookup"><span data-stu-id="05ecd-115">If necessary, switch to a different subscription.</span></span> <span data-ttu-id="05ecd-116">[了解如何](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)操作。</span><span class="sxs-lookup"><span data-stu-id="05ecd-116">[Learn how](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).</span></span>
3.    <span data-ttu-id="05ecd-117">如果已使用任何其他 Microsoft 订阅在 RDS 服务器上安装了 Office，请将其卸载。</span><span class="sxs-lookup"><span data-stu-id="05ecd-117">If Office is already installed on the RDS server using any other Microsoft subscriptions, uninstall it.</span></span> <span data-ttu-id="05ecd-118">例如，转到 **"控制面板"**  >  **卸载程序**。</span><span class="sxs-lookup"><span data-stu-id="05ecd-118">For example, by going to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="05ecd-119">如果遇到问题，请使用 [Microsoft 支持和恢复助手](https://aka.ms/SARA-OfficeUninstall-Alchemy) 卸载。</span><span class="sxs-lookup"><span data-stu-id="05ecd-119">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>
4.    <span data-ttu-id="05ecd-120">在 RDS 服务器上，使用管理员帐户登录 Microsoft 365 管理中心并 [安装适用于企业的 microsoft 365 应用程序](https://portal.office.com/OLS/MySoftware.aspx)。</span><span class="sxs-lookup"><span data-stu-id="05ecd-120">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
5.    <span data-ttu-id="05ecd-121">安装 Office 后，请 ***不要打开或登录*** 任何 Office 应用程序。</span><span class="sxs-lookup"><span data-stu-id="05ecd-121">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>
6.    <span data-ttu-id="05ecd-122">在 RDS 服务器上，通过执行以下步骤，通过编辑注册表来启用共享计算机激活：</span><span class="sxs-lookup"><span data-stu-id="05ecd-122">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
   1. <span data-ttu-id="05ecd-123">右键单击屏幕左下角的 "Windows" 按钮，然后选择 " **运行**"。</span><span class="sxs-lookup"><span data-stu-id="05ecd-123">Right-click the Windows button in the lower left-corner of your screen and select **Run**.</span></span> <span data-ttu-id="05ecd-124">在 "打开" 框中，键入 " **regedit**"，然后选择 **"确定"**。</span><span class="sxs-lookup"><span data-stu-id="05ecd-124">In the Open box, type **regedit**, and then select **OK**.</span></span>
   2. <span data-ttu-id="05ecd-125">当系统提示允许注册表编辑器对设备进行更改时，选择 **"是"** 。</span><span class="sxs-lookup"><span data-stu-id="05ecd-125">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
   3. <span data-ttu-id="05ecd-126">在注册表编辑器中，在 HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration. 下添加 **SharedComputerLicensing** 的字符串值设置为1。</span><span class="sxs-lookup"><span data-stu-id="05ecd-126">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>
   4. <span data-ttu-id="05ecd-127">在 RDS 服务器上， ***以最终用户的形式登录*** ，并 [验证是否已为 Microsoft 365 的企业版应用程序激活共享计算机激活](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)。</span><span class="sxs-lookup"><span data-stu-id="05ecd-127">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

