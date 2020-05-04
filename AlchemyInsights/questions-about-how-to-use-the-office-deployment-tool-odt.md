---
title: 有关如何使用 Office 部署工具（ODT）的问题
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 4aef42df4dde17d15863fca67e41f0ff23e506dc
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010721"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="9ae20-102">有关如何使用 Office 部署工具（ODT）的问题</span><span class="sxs-lookup"><span data-stu-id="9ae20-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="9ae20-103">[从 Microsoft 下载中心](https://go.microsoft.com/fwlink/p/?LinkID=626065)下载 Office 部署工具。</span><span class="sxs-lookup"><span data-stu-id="9ae20-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="9ae20-104">下载文件后，运行自解压缩可执行文件，其中包含 Office 部署工具可执行文件 (setup.exe) 和一个示例配置文件 (configuration.xml)。</span><span class="sxs-lookup"><span data-stu-id="9ae20-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="9ae20-105">**若要从客户端计算机中排除或删除适用于企业产品的 Microsoft 365 应用程序：**</span><span class="sxs-lookup"><span data-stu-id="9ae20-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="9ae20-106">在安装适用于企业的 Microsoft 365 应用程序时，您可以排除特定产品。</span><span class="sxs-lookup"><span data-stu-id="9ae20-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="9ae20-107">若要执行此操作，请按照使用 ODT 安装 Office 的步骤操作，但请将 ExcludeApp 元素包括在配置文件中。</span><span class="sxs-lookup"><span data-stu-id="9ae20-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="9ae20-108">例如，此配置文件将安装除 Publisher 之外的所有适用于企业产品的 Microsoft 365 应用程序：</span><span class="sxs-lookup"><span data-stu-id="9ae20-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="9ae20-109">Office 部署工具概述</span><span class="sxs-lookup"><span data-stu-id="9ae20-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

