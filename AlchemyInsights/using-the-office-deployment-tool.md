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
ms.openlocfilehash: 39a011d4b121492d222ff620e70d9860231b7bcfe0d7fd2ecfd93de1ef502f5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083760"
---
# <a name="using-the-office-deployment-tool-odt"></a>使用 Office 部署工具 (ODT) 

使用 ODT Office部署 (部署) 部署Office 365部署Office。 The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.
  
1. 从 Microsoft 下载中心下载 Office 部署[工具的最新版本](https://go.microsoft.com/fwlink/p/?LinkID=626065)。

2. 使用[OCT Office自定义 (工具) ](https://config.office.com)选择部署首选项并创建配置 XML 文件。 导出配置文件，并本地放置到文件所在的setup.exe文件夹。

    **注意：Office** 配置不正确或格式不正确的配置文件，通常会出现安装问题。 为了避免此类问题，建议您使用自定义Office工具创建配置文件。 还可以将现有配置文件导入到自定义Office工具中。

3. 从提升的命令提示符下，切换到 setup.exe 所在的位置，在下载模式下运行 Office 部署工具，并指定刚保存的配置文件。 此示例将配置文件命名为 Configuration.xml：

```setup.exe /download Configuration.xml```

4.在Office运行部署工具并指定配置文件。

```setup.exe /configure Configuration.xml```

**注意：** 必须从要安装数据库的客户端计算机中运行此步骤Office并且必须具有该计算机的本地管理员权限。

若要了解有关将 Office 部署工具用于 Microsoft 365 企业应用版 部署方案Office[概述](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)。 有关如何使用自定义工具的Office，请参阅自定义[工具Office概述](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)。
