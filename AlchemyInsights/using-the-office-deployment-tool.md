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
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2019
ms.locfileid: "28277720"
---
# <a name="using-the-office-deployment-tool-odt"></a>Using the Office Deployment Tool (ODT)

使用 Office 部署工具 (ODT) 来部署 Office 365 版本的 Office。Office 部署工具 (setup.exe) 从命令行运行并使用 XML 配置文件来确定要部署 Office 时应用设置。
  
1. 从[Microsoft 下载中心](http://go.microsoft.com/fwlink/p/?LinkID=626065)下载最新版本的 Office 部署工具。
    
2. 使用[Office 自定义工具 (OCT)](https://config.office.com)选择部署首选项并创建 XML 配置文件。导出配置文件并将其放置本地 setup.exe 所在的同一个文件夹。 
    
    **注意：** Office 安装通常会发生问题截止到配置不正确或格式错误配置文件。若要避免此类问题，我们建议您使用 Office 自定义工具以创建配置文件。您还可以导入 Office 自定义工具的现有配置文件。 
    
3. 从提升的命令提示符处，切换到 setup.exe 所在的位置，以 download 模式运行 Office 部署工具，并指定您刚才保存的配置文件。此示例中，在配置文件被命名为 Configuration.xml:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. 运行 Office 部署工具中配置模式并指定配置文件。
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **注意：** 您必须从客户端计算机要安装 Office，并且您必须本地管理员权限的计算机上运行此步骤。 
    
若要了解有关为 Office 365 ProPlus 部署方案中使用 Office 部署工具的详细信息，请参阅[Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)。有关如何使用 Office 自定义工具的详细信息，请参阅[Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)。
  

