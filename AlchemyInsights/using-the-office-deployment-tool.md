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
# <a name="using-the-office-deployment-tool-odt"></a>使用 Office 部署工具 (ODT) 

您可以使用 Office 部署工具 (ODT) 部署 office 365 版本的 Office。 Office 部署工具 ( # A0) 从命令行运行，并使用配置 XML 文件确定在部署 Office 时要应用的设置。
  
1. 从 [Microsoft 下载中心](https://go.microsoft.com/fwlink/p/?LinkID=626065)下载 Office 部署工具的最新版本。

2. 使用 [Office 自定义工具 (OCT) ](https://config.office.com) 选择您的部署首选项并创建配置 XML 文件。 导出配置文件，并将其放在 setupodt.exe 所在的同一文件夹中。

    **注意：** Office 安装问题通常是由于配置不正确或 malformatted 配置文件导致的。 若要避免此类问题，建议使用 Office 自定义工具创建配置文件。 您还可以将现有配置文件导入 Office 自定义工具。

3. 从提升的命令提示符处，切换到 setupodt.exe 所在的位置，并在下载模式下运行 Office 部署工具，并指定刚保存的配置文件。 在此示例中，配置文件命名为 Configuration.xml：

```setupodt.exe /download Configuration.xml```

4. 在 "配置" 模式下运行 Office 部署工具并指定配置文件。

```setupodt.exe /configure Configuration.xml```

**注意：** 必须在要安装 Office 的客户端计算机上运行此步骤，并且必须具有该计算机的本地管理员权限。

若要详细了解如何使用适用于 Microsoft 365 应用程序的 Office 部署工具进行企业级部署方案，请参阅 [Office 部署工具概述](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)。 有关如何使用 Office 自定义工具的详细信息，请参阅 [Office 自定义工具概述](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)。
