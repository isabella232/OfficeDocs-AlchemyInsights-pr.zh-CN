---
title: 使用 Office 部署工具
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: f3a5dbfc6b64ccd4f0b19a5f86236336e78838d4
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085822"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="06488-102">使用 Office 部署工具 (ODT) </span><span class="sxs-lookup"><span data-stu-id="06488-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="06488-103">您可以使用 Office 部署工具 (ODT) 部署 office 365 版本的 Office。</span><span class="sxs-lookup"><span data-stu-id="06488-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="06488-104">Office 部署工具 ( # A0) 从命令行运行，并使用配置 XML 文件确定在部署 Office 时要应用的设置。</span><span class="sxs-lookup"><span data-stu-id="06488-104">The Office Deployment Tool (setupodt.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="06488-105">从 [Microsoft 下载中心](https://go.microsoft.com/fwlink/p/?LinkID=626065)下载 Office 部署工具的最新版本。</span><span class="sxs-lookup"><span data-stu-id="06488-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="06488-106">使用 [Office 自定义工具 (OCT) ](https://config.office.com) 选择您的部署首选项并创建配置 XML 文件。</span><span class="sxs-lookup"><span data-stu-id="06488-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="06488-107">导出配置文件，并将其放在 setupodt.exe 所在的同一文件夹中。</span><span class="sxs-lookup"><span data-stu-id="06488-107">Export the configuration file and place it locally on the same folder where the setupodt.exe resides.</span></span>

    <span data-ttu-id="06488-108">**注意：** Office 安装问题通常是由于配置不正确或 malformatted 配置文件导致的。</span><span class="sxs-lookup"><span data-stu-id="06488-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="06488-109">若要避免此类问题，建议使用 Office 自定义工具创建配置文件。</span><span class="sxs-lookup"><span data-stu-id="06488-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="06488-110">您还可以将现有配置文件导入 Office 自定义工具。</span><span class="sxs-lookup"><span data-stu-id="06488-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="06488-111">从提升的命令提示符处，切换到 setupodt.exe 所在的位置，并在下载模式下运行 Office 部署工具，并指定刚保存的配置文件。</span><span class="sxs-lookup"><span data-stu-id="06488-111">From an elevated command prompt, switch to the location where setupodt.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="06488-112">在此示例中，配置文件命名为 Configuration.xml：</span><span class="sxs-lookup"><span data-stu-id="06488-112">In this example, the configuration file is named Configuration.xml:</span></span>

```setupodt.exe /download Configuration.xml```

<span data-ttu-id="06488-113">4. 在 "配置" 模式下运行 Office 部署工具并指定配置文件。</span><span class="sxs-lookup"><span data-stu-id="06488-113">4.Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>

```setupodt.exe /configure Configuration.xml```

<span data-ttu-id="06488-114">**注意：** 必须在要安装 Office 的客户端计算机上运行此步骤，并且必须具有该计算机的本地管理员权限。</span><span class="sxs-lookup"><span data-stu-id="06488-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="06488-115">若要详细了解如何使用适用于 Microsoft 365 应用程序的 Office 部署工具进行企业级部署方案，请参阅 [Office 部署工具概述](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)。</span><span class="sxs-lookup"><span data-stu-id="06488-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span></span> <span data-ttu-id="06488-116">有关如何使用 Office 自定义工具的详细信息，请参阅 [Office 自定义工具概述](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)。</span><span class="sxs-lookup"><span data-stu-id="06488-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
