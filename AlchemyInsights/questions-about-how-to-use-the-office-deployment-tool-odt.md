---
title: 有关如何使用 Office 部署工具 (ODT) 的问题
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: c16b7ac7d79794307fa33ed1039305ed5b842cf6
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2019
ms.locfileid: "28276875"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="e81c4-102">有关如何使用 Office 部署工具 (ODT) 的问题</span><span class="sxs-lookup"><span data-stu-id="e81c4-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="e81c4-103">[从 Microsoft 下载中心](http://go.microsoft.com/fwlink/p/?LinkID=626065)下载 Office 部署工具。</span><span class="sxs-lookup"><span data-stu-id="e81c4-103">Download the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="e81c4-104">下载文件后，运行自解压缩可执行文件，其中包含 Office 部署工具可执行文件 (setup.exe) 和一个示例配置文件 (configuration.xml)。</span><span class="sxs-lookup"><span data-stu-id="e81c4-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="e81c4-105">**排除或从客户端计算机中删除 Office 365 ProPlus 的产品：**</span><span class="sxs-lookup"><span data-stu-id="e81c4-105">**To exclude or remove Office 365 ProPlus products from client computers:**</span></span>
  
<span data-ttu-id="e81c4-p101">安装 Office 365 ProPlus 时可以排除特定的产品。若要执行此操作，请按照使用 ODT 安装 Office 的步骤，但是将 ExcludeApp 元素包括在你的配置文件中。例如，此配置文件安装除 Publisher 以外的所有 Office 365 ProPlus 产品。</span><span class="sxs-lookup"><span data-stu-id="e81c4-p101">When installing Office 365 ProPlus, you can exclude specific products. To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file. For example, this configuration file installs all the Office 365 ProPlus products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="e81c4-109">Office 部署工具概述</span><span class="sxs-lookup"><span data-stu-id="e81c4-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

