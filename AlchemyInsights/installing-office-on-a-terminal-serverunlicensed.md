---
title: 在终端服务器上安装 office-未授权
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663107"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="a8ef9-102">在终端服务器上安装 Office</span><span class="sxs-lookup"><span data-stu-id="a8ef9-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="a8ef9-103">若要在使用远程桌面服务的 Windows 服务器上部署适用于企业的 Microsoft 365 应用程序 (RDS) （以前称为 "终端服务"）：</span><span class="sxs-lookup"><span data-stu-id="a8ef9-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="a8ef9-104">您必须拥有包含适用于企业的 Microsoft 365 应用程序的 Microsoft 365 订阅，例如 Office 365 企业版 E3 或企业版 E5。</span><span class="sxs-lookup"><span data-stu-id="a8ef9-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="a8ef9-105">适用于商业的 Microsoft 365 apps 和 Microsoft 365 应用程序高级计划不包含适用于企业的 Microsoft 365 应用程序。</span><span class="sxs-lookup"><span data-stu-id="a8ef9-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="a8ef9-106">您需要启用 [共享计算机激活](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)。</span><span class="sxs-lookup"><span data-stu-id="a8ef9-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

<span data-ttu-id="a8ef9-107">如果要从 Microsoft 365 管理中心（ ***使用默认安装设置***）在 RDS 上安装 Microsoft 365 应用程序，请执行以下步骤。</span><span class="sxs-lookup"><span data-stu-id="a8ef9-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="a8ef9-108">您还可以下载并运行 [Microsoft 支持和恢复助理](https://aka.ms/SaRA_OfficeSCA_M365Portal) ，以在共享计算机激活模式下安装适用于企业的 Microsoft 365 应用程序。</span><span class="sxs-lookup"><span data-stu-id="a8ef9-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="a8ef9-109">检查您拥有的 Microsoft 365 订阅。</span><span class="sxs-lookup"><span data-stu-id="a8ef9-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="a8ef9-110">了解方法</span><span class="sxs-lookup"><span data-stu-id="a8ef9-110">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="a8ef9-111">如有必要，请切换到其他 Microsoft 365 订阅。</span><span class="sxs-lookup"><span data-stu-id="a8ef9-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="a8ef9-112">了解方法</span><span class="sxs-lookup"><span data-stu-id="a8ef9-112">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. <span data-ttu-id="a8ef9-113">如果已使用任何其他 Microsoft 365 订阅在 RDS 服务器上安装了 Office，请将其卸载。</span><span class="sxs-lookup"><span data-stu-id="a8ef9-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="a8ef9-114">例如，转到 "控制面板" \> 卸载程序。</span><span class="sxs-lookup"><span data-stu-id="a8ef9-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="a8ef9-115">如果遇到问题，请使用 [Microsoft 支持和恢复助手](https://aka.ms/SARA-OfficeUninstall-Alchemy) 卸载。</span><span class="sxs-lookup"><span data-stu-id="a8ef9-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="a8ef9-116">在 RDS 服务器上，使用管理员帐户登录 Microsoft 365 管理中心并 [安装适用于企业的 microsoft 365 应用程序](https://portal.office.com/OLS/MySoftware.aspx)。</span><span class="sxs-lookup"><span data-stu-id="a8ef9-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="a8ef9-117">安装 Office 后，请 ***不要打开或登录*** 任何 Office 应用程序。</span><span class="sxs-lookup"><span data-stu-id="a8ef9-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="a8ef9-118">在 RDS 服务器上，通过执行以下步骤，通过编辑注册表来启用共享计算机激活：</span><span class="sxs-lookup"><span data-stu-id="a8ef9-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="a8ef9-119">右键单击屏幕左下角的 "Windows" 按钮，然后选择 "运行"。</span><span class="sxs-lookup"><span data-stu-id="a8ef9-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="a8ef9-120">在 "打开" 框中，键入 " **regedit**"，然后选择 "确定"。</span><span class="sxs-lookup"><span data-stu-id="a8ef9-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="a8ef9-121">当系统提示允许注册表编辑器对设备进行更改时，选择 "是"。</span><span class="sxs-lookup"><span data-stu-id="a8ef9-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="a8ef9-122">在注册表编辑器中，在 HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration. 下添加 **SharedComputerLicensing** 的字符串值设置为1。</span><span class="sxs-lookup"><span data-stu-id="a8ef9-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="a8ef9-123">在 RDS 服务器上， ***以最终用户的形式登录*** ，并 [验证是否已为 Microsoft 365 的企业版应用程序激活共享计算机激活](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)。</span><span class="sxs-lookup"><span data-stu-id="a8ef9-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

<span data-ttu-id="a8ef9-124">有关使用 Office 部署工具的自定义安装的先决条件、设置说明和指南的详细信息，请参阅 [Deploy Microsoft 365 Apps for enterprise by Using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)。</span><span class="sxs-lookup"><span data-stu-id="a8ef9-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>
  
<span data-ttu-id="a8ef9-125">若要修复与共享计算机激活相关的错误，请参阅 [针对企业共享计算机激活的 Microsoft 365 应用程序的故障排除问题](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)。</span><span class="sxs-lookup"><span data-stu-id="a8ef9-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
  