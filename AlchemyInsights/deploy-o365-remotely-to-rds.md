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
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="6b1dd-102">部署 Microsoft 365 企业应用版以在 RDS、终端服务器或 VDI 上共享使用</span><span class="sxs-lookup"><span data-stu-id="6b1dd-102">Deploying Microsoft 365 Apps for enterprise for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="6b1dd-103">若要使用远程桌面服务部署 Microsoft 365 企业应用版， (RDS) 以前称为终端服务：</span><span class="sxs-lookup"><span data-stu-id="6b1dd-103">To deploy Microsoft 365 Apps for enterprise using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>

- <span data-ttu-id="6b1dd-104">必须具有 Microsoft 365 商业版计划或包含 Microsoft 365 企业应用版（如 Office 365 企业版 E3 或企业版 E5）的 Office 365 计划。</span><span class="sxs-lookup"><span data-stu-id="6b1dd-104">You must have a Microsoft 365 For Business plan or an Office 365 plan that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span>
   > [!NOTE]
   > <span data-ttu-id="6b1dd-105">Microsoft 365 商业应用版和 Microsoft 365 商业标准版计划不包括 Microsoft 365 企业应用版。</span><span class="sxs-lookup"><span data-stu-id="6b1dd-105">The Microsoft 365 Apps for business and Microsoft 365 Business Standard plans do not include Microsoft 365 Apps for enterprise.</span></span>
- <span data-ttu-id="6b1dd-106">必须启用 [共享计算机激活](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)。</span><span class="sxs-lookup"><span data-stu-id="6b1dd-106">You must enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

> [!NOTE]
> <span data-ttu-id="6b1dd-107">还可以下载并运行 Microsoft [支持和恢复助手](https://aka.ms/SaRA_OfficeSCA_M365Portal) ，以在共享计算机激活模式下安装 Microsoft 365 企业应用版。</span><span class="sxs-lookup"><span data-stu-id="6b1dd-107">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>

<span data-ttu-id="6b1dd-108">有关使用 Office 部署工具的自定义安装的先决条件、设置说明和指南详细信息，请参阅使用远程桌面服务部署 [Microsoft 365](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)企业应用版。</span><span class="sxs-lookup"><span data-stu-id="6b1dd-108">For more information on prerequisites, setup instructions, and guidance on customized installations by using the Office Deployment Tool, see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>

<span data-ttu-id="6b1dd-109">若要修复与共享计算机激活相关的错误，</span><span class="sxs-lookup"><span data-stu-id="6b1dd-109">To fix errors related to shared computer activation:</span></span>

- <span data-ttu-id="6b1dd-110">请参阅 [排查 Microsoft 365](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)企业应用版共享计算机激活问题。</span><span class="sxs-lookup"><span data-stu-id="6b1dd-110">See [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
- <span data-ttu-id="6b1dd-111">参见[重置 Microsoft 365 企业版应用激活状态](https://go.microsoft.com/fwlink/?linkid=2109218)。</span><span class="sxs-lookup"><span data-stu-id="6b1dd-111">See [Reset Microsoft 365 Apps for enterprise activation state](https://go.microsoft.com/fwlink/?linkid=2109218).</span></span>

<span data-ttu-id="6b1dd-112">如果要从使用默认安装设置的 Microsoft 365 管理中心在 RDS 上安装 Microsoft 365 企业应用版，请使用以下步骤：</span><span class="sxs-lookup"><span data-stu-id="6b1dd-112">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps:</span></span>

1. <span data-ttu-id="6b1dd-113">检查你拥有哪些订阅。</span><span class="sxs-lookup"><span data-stu-id="6b1dd-113">Check what subscription you have.</span></span> <span data-ttu-id="6b1dd-114">[了解如何。](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)</span><span class="sxs-lookup"><span data-stu-id="6b1dd-114">[Learn how](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).</span></span>
2. <span data-ttu-id="6b1dd-115">如有必要，切换到其他订阅。</span><span class="sxs-lookup"><span data-stu-id="6b1dd-115">If necessary, switch to a different subscription.</span></span> <span data-ttu-id="6b1dd-116">[了解如何。](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)</span><span class="sxs-lookup"><span data-stu-id="6b1dd-116">[Learn how](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).</span></span>
3. <span data-ttu-id="6b1dd-117">如果 RDS 服务器上已经使用任何其他 Microsoft 订阅安装了 Office，请卸载它。</span><span class="sxs-lookup"><span data-stu-id="6b1dd-117">If Office is already installed on the RDS server using any other Microsoft subscriptions, uninstall it.</span></span> <span data-ttu-id="6b1dd-118">例如，通过进入控制面板 **卸载**  >  **程序**。</span><span class="sxs-lookup"><span data-stu-id="6b1dd-118">For example, by going to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="6b1dd-119">如果正在运行 [问题，](https://aka.ms/SARA-OfficeUninstall-Alchemy) 使用 Microsoft 支持和恢复助手卸载。</span><span class="sxs-lookup"><span data-stu-id="6b1dd-119">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>
4. <span data-ttu-id="6b1dd-120">在 RDS 服务器上，使用管理员帐户登录到 Microsoft 365 管理中心，然后安装 [Microsoft 365 企业应用版](https://portal.office.com/OLS/MySoftware.aspx)。</span><span class="sxs-lookup"><span data-stu-id="6b1dd-120">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
5. <span data-ttu-id="6b1dd-121">安装 Office 后 ***，不要打开或登录任何*** Office 应用程序。</span><span class="sxs-lookup"><span data-stu-id="6b1dd-121">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>
6. <span data-ttu-id="6b1dd-122">在 RDS 服务器上，通过按照以下步骤编辑注册表来启用共享计算机激活：</span><span class="sxs-lookup"><span data-stu-id="6b1dd-122">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
   1. <span data-ttu-id="6b1dd-123">右键单击屏幕左下角的 Windows 按钮， **然后选择运行**。</span><span class="sxs-lookup"><span data-stu-id="6b1dd-123">Right-click the Windows button in the lower left-corner of your screen and select **Run**.</span></span> <span data-ttu-id="6b1dd-124">在"打开"框中，键入 **regedit**，然后选择"确定 **"。**</span><span class="sxs-lookup"><span data-stu-id="6b1dd-124">In the Open box, type **regedit**, and then select **OK**.</span></span>
   2. <span data-ttu-id="6b1dd-125">当 **系统** 提示允许注册表编辑器对设备进行更改时，选择"是"。</span><span class="sxs-lookup"><span data-stu-id="6b1dd-125">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
   3. <span data-ttu-id="6b1dd-126">在注册表编辑器中，将 **SharedComputerLicensing** 的字符串值添加到 HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration 下，将设置为 1。</span><span class="sxs-lookup"><span data-stu-id="6b1dd-126">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>
   4. <span data-ttu-id="6b1dd-127">在 RDS 服务器上 ***，以*** 最终用户身份登录并验证共享计算机激活是否已启用 [Microsoft 365 企业应用版](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)。</span><span class="sxs-lookup"><span data-stu-id="6b1dd-127">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>
