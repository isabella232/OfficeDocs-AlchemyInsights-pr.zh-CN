---
title: 使用 Office 部署工具
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: b4ade0f21794a8986aa7a37d783da5fa289488fc
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29459225"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="337f6-102">Using the Office Deployment Tool (ODT)</span><span class="sxs-lookup"><span data-stu-id="337f6-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="337f6-p101">使用 Office 部署工具 (ODT) 来部署 Office 365 版本的 Office。Office 部署工具 (setup.exe) 从命令行运行并使用 XML 配置文件来确定要部署 Office 时应用设置。</span><span class="sxs-lookup"><span data-stu-id="337f6-p101">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office. The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="337f6-105">从[Microsoft 下载中心](http://go.microsoft.com/fwlink/p/?LinkID=626065)下载最新版本的 Office 部署工具。</span><span class="sxs-lookup"><span data-stu-id="337f6-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
    
2. <span data-ttu-id="337f6-p102">使用[Office 自定义工具 (OCT)](https://config.office.com)选择部署首选项并创建 XML 配置文件。导出配置文件并将其放置本地 setup.exe 所在的同一个文件夹。</span><span class="sxs-lookup"><span data-stu-id="337f6-p102">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file. Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span> 
    
    <span data-ttu-id="337f6-p103">**注意：** Office 安装通常会发生问题截止到配置不正确或格式错误配置文件。若要避免此类问题，我们建议您使用 Office 自定义工具以创建配置文件。您还可以导入 Office 自定义工具的现有配置文件。</span><span class="sxs-lookup"><span data-stu-id="337f6-p103">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files. To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file. You can also import existing configuration files into the Office Customization Tool.</span></span> 
    
3. <span data-ttu-id="337f6-p104">从提升的命令提示符处，切换到 setup.exe 所在的位置，以 download 模式运行 Office 部署工具，并指定您刚才保存的配置文件。此示例中，在配置文件被命名为 Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="337f6-p104">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved. In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="337f6-113">运行 Office 部署工具中配置模式并指定配置文件。</span><span class="sxs-lookup"><span data-stu-id="337f6-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="337f6-114">**注意：** 您必须从客户端计算机要安装 Office，并且您必须本地管理员权限的计算机上运行此步骤。</span><span class="sxs-lookup"><span data-stu-id="337f6-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span> 
    
<span data-ttu-id="337f6-p105">若要了解有关为 Office 365 ProPlus 部署方案中使用 Office 部署工具的详细信息，请参阅[Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)。有关如何使用 Office 自定义工具的详细信息，请参阅[Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)。</span><span class="sxs-lookup"><span data-stu-id="337f6-p105">To learn more about using Office Deployment Tool for your Office 365 ProPlus deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
  

