---
title: 使用 Office 部署工具
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: 874bb7883bca4f062e85963a6828a771cd2dad9b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36531565"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="aec92-102">使用 Office 部署工具 (ODT)</span><span class="sxs-lookup"><span data-stu-id="aec92-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="aec92-103">您可以使用 Office 部署工具 (ODT) 部署 Office 365 版本的 Office。</span><span class="sxs-lookup"><span data-stu-id="aec92-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="aec92-104">Office 部署工具 (setup.exe) 从命令行运行, 并使用配置 XML 文件确定部署 Office 时要应用的设置。</span><span class="sxs-lookup"><span data-stu-id="aec92-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="aec92-105">从[Microsoft 下载中心](http://go.microsoft.com/fwlink/p/?LinkID=626065)下载 Office 部署工具的最新版本。</span><span class="sxs-lookup"><span data-stu-id="aec92-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="aec92-106">使用[Office 自定义工具 (OCT)](https://config.office.com)选择您的部署首选项并创建配置 XML 文件。</span><span class="sxs-lookup"><span data-stu-id="aec92-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="aec92-107">导出配置文件, 并将其放置在 setup.exe 所在的同一文件夹中。</span><span class="sxs-lookup"><span data-stu-id="aec92-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span>

    <span data-ttu-id="aec92-108">**注意:** Office 安装问题通常是由于配置不正确或 malformatted 配置文件导致的。</span><span class="sxs-lookup"><span data-stu-id="aec92-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="aec92-109">若要避免此类问题, 建议使用 Office 自定义工具创建配置文件。</span><span class="sxs-lookup"><span data-stu-id="aec92-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="aec92-110">您还可以将现有配置文件导入 Office 自定义工具。</span><span class="sxs-lookup"><span data-stu-id="aec92-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="aec92-111">从提升的命令提示符处, 切换到 setup.exe 所在的位置, 并在下载模式下运行 Office 部署工具, 并指定刚保存的配置文件。</span><span class="sxs-lookup"><span data-stu-id="aec92-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="aec92-112">在此示例中, 配置文件命名为 config.xml:</span><span class="sxs-lookup"><span data-stu-id="aec92-112">In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="aec92-113">在 "配置" 模式下运行 Office 部署工具并指定配置文件。</span><span class="sxs-lookup"><span data-stu-id="aec92-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="aec92-114">**注意:** 必须在要安装 Office 的客户端计算机上运行此步骤, 并且必须具有该计算机的本地管理员权限。</span><span class="sxs-lookup"><span data-stu-id="aec92-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="aec92-115">若要了解有关为 Office 365 专业增强版部署方案使用 Office 部署工具的详细信息, 请参阅[Office 部署工具概述](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)。</span><span class="sxs-lookup"><span data-stu-id="aec92-115">To learn more about using Office Deployment Tool for your Office 365 ProPlus deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span></span> <span data-ttu-id="aec92-116">有关如何使用 Office 自定义工具的详细信息, 请参阅[Office 自定义工具概述](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)。</span><span class="sxs-lookup"><span data-stu-id="aec92-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
