---
title: 有关如何使用 Office 部署工具 (ODT) 的问题
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: c5b055989014b464d3136895702c8ea40e8eb701
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086146"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="cfcb3-102">有关如何使用 Office 部署工具 (ODT) 的问题</span><span class="sxs-lookup"><span data-stu-id="cfcb3-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="cfcb3-103">[从 Microsoft 下载中心](https://go.microsoft.com/fwlink/p/?LinkID=626065)下载 Office 部署工具。</span><span class="sxs-lookup"><span data-stu-id="cfcb3-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="cfcb3-104">下载文件后，运行自解压缩可执行文件，其中包含 ( # A0) 的 Office 部署工具可执行文件和) # A1 的示例配置文件 (。</span><span class="sxs-lookup"><span data-stu-id="cfcb3-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setupodt.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="cfcb3-105">**若要从客户端计算机中排除或删除适用于企业产品的 Microsoft 365 应用程序：**</span><span class="sxs-lookup"><span data-stu-id="cfcb3-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="cfcb3-106">在安装适用于企业的 Microsoft 365 应用程序时，您可以排除特定产品。</span><span class="sxs-lookup"><span data-stu-id="cfcb3-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="cfcb3-107">若要执行此操作，请按照使用 ODT 安装 Office 的步骤操作，但请将 ExcludeApp 元素包括在配置文件中。</span><span class="sxs-lookup"><span data-stu-id="cfcb3-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="cfcb3-108">例如，此配置文件将安装除 Publisher 之外的所有适用于企业产品的 Microsoft 365 应用程序：</span><span class="sxs-lookup"><span data-stu-id="cfcb3-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="cfcb3-109">Office 部署工具概述</span><span class="sxs-lookup"><span data-stu-id="cfcb3-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

