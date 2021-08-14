---
title: '有关如何使用 ODT Office部署 (的问题) '
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: d38866647c7bf286b5b5b21e7fdcc94af72ea1850bc40391af077aa230b8b4fd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959673"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>有关如何使用 ODT Office部署 (的问题) 

[从 Microsoft 下载中心](https://go.microsoft.com/fwlink/p/?LinkID=626065)下载 Office 部署工具。
  
下载文件后，运行自解压缩可执行文件，其中包含 Office 部署工具可执行文件 (setup.exe) 和一个示例配置文件 (configuration.xml)。
  
 **若要从客户端计算机Microsoft 365 企业应用版或删除产品：**
  
在安装Microsoft 365 企业应用版时，可以排除特定产品。 若要执行此操作，请按照使用 ODT 安装 Office 的步骤操作，但请将 ExcludeApp 元素包括在配置文件中。 例如，此配置文件将安装除以下Microsoft 365 企业应用版产品Publisher：
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Office 部署工具概述](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

