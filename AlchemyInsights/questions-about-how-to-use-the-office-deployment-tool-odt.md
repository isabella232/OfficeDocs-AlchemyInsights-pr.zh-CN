---
title: '有关如何使用 Office 部署工具 (ODT) '
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
ms.openlocfilehash: 20e0b6aa3c298ee0a4291c3da6ae46978177e81f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790322"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>有关如何使用 Office 部署工具 (ODT) 

[从 Microsoft 下载中心](https://go.microsoft.com/fwlink/p/?LinkID=626065)下载 Office 部署工具。
  
下载文件后，运行自解压缩可执行文件，其中包含 Office 部署工具可执行文件 (setup.exe) 和一个示例配置文件 (configuration.xml)。
  
 **若要从客户端计算机中排除或删除 Microsoft 365 企业应用版产品：：**
  
安装 Microsoft 365 企业应用版时，可以排除特定产品。 若要执行此操作，请按照使用 ODT 安装 Office 的步骤操作，但请将 ExcludeApp 元素包括在配置文件中。 例如，此配置文件将安装除 Publisher 之外的所有 Microsoft 365 企业应用版产品：
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Office 部署工具概述](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

