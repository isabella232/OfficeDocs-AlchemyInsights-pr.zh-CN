---
title: 管理 SharePoint Online 中的搜索架构
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 8eb0e93ea5bbf2154213274041b28a3c908090dae724b8f8e55fa2fb05f16d86
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54085074"
---
# <a name="manage-search-schema-in-sharepoint-online"></a>管理 SharePoint Online 中的搜索架构

搜索架构控制用户可以搜索的内容、用户搜索方式以及如何在搜索网站上显示结果。 

请参阅[管理 SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema)中的搜索架构，了解如何： 
- 更改搜索架构。
- 创建托管属性。
- 将已爬网映射的已爬网属性映射到托管属性。

关于管理搜索架构，请注意以下几点：

- 如果您收到一 **条警告，** 指出在更改架构时应用程序已暂停，这仅仅是临时的，因为发生服务维护。 

    如果超过 24 小时，但仍遇到警告，请记录支持案例。
- 当您更改托管属性或添加新属性时，更改仅在重新爬网内容后生效。 在 SharePoint Online 中，根据定义的爬网计划自动进行爬网。
- 若要确保对更改进行爬网，可以专门请求对列表或库重新 [编制索引](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list) 

有关搜索架构的完整概述，请参阅 [介绍搜索架构](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/) 


