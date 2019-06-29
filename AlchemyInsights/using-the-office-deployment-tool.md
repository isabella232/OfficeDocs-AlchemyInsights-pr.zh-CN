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
ms.openlocfilehash: 998f914f38fa9d1925f7003e634d7f11550f47da
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/28/2019
ms.locfileid: "35365515"
---
# <a name="using-the-office-deployment-tool-odt"></a>使用 Office 部署工具 (ODT)

您可以使用 Office 部署工具 (ODT) 部署 Office 365 版本的 Office。 Office 部署工具 (setup.exe) 从命令行运行, 并使用配置 XML 文件确定部署 Office 时要应用的设置。
  
1. 从[Microsoft 下载中心](http://go.microsoft.com/fwlink/p/?LinkID=626065)下载 Office 部署工具的最新版本。

2. 使用[Office 自定义工具 (OCT)](https://config.office.com)选择您的部署首选项并创建配置 XML 文件。 导出配置文件, 并将其放置在 setup.exe 所在的同一文件夹中。

    **注意:** Office 安装问题通常是由于配置不正确或 malformatted 配置文件导致的。 若要避免此类问题, 建议使用 Office 自定义工具创建配置文件。 您还可以将现有配置文件导入 Office 自定义工具。

3. 从提升的命令提示符处, 切换到 setup.exe 所在的位置, 并在下载模式下运行 Office 部署工具, 并指定刚保存的配置文件。 在此示例中, 配置文件命名为 config.xml:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. 在 "配置" 模式下运行 Office 部署工具并指定配置文件。
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **注意:** 必须在要安装 Office 的客户端计算机上运行此步骤, 并且必须具有该计算机的本地管理员权限。

若要了解有关为 Office 365 专业增强版部署方案使用 Office 部署工具的详细信息, 请参阅[Office 部署工具概述](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)。 有关如何使用 Office 自定义工具的详细信息, 请参阅[Office 自定义工具概述](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)。
