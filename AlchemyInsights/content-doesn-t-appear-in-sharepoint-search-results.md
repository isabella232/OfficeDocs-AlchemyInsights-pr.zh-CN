---
title: 内容未显示在 SharePoint 搜索结果中
ms.author: tlarsen
author: tklarsen
ms.date: 1/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: 8215b0a5cde5adffa3bec37d6699418557f914dd
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/28/2019
ms.locfileid: "35363788"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>内容未显示在 SharePoint 搜索结果中

在搜索结果中不显示预期内容时, 请按照以下疑难解答步骤进行操作:
  
1. 检查包含预期内容的**网站**是否设置为允许内容显示在搜索结果中。 按照在[搜索结果中显示网站上的内容](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results)中的步骤操作。

2. 检查包含预期内容的**列表**或**库**是否设置为允许内容显示在搜索结果中。 按照 "在[搜索结果中显示列表或库](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results)中的内容" 中的步骤操作。

3. 验证页面、文档或自定义页面布局是否已发布为**主要版本。** 执行搜索中的步骤 3[不会在 SharePoint Online 中返回所有结果](https://go.microsoft.com/fwlink/?linkid=874525)。

4. 验证用户是否具有查看内容的**权限**。 按照[了解 SharePoint 中的权限级别](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels)中的步骤操作。
    
5. 如果已通过添加新的托管属性、编辑托管属性或删除托管属性来更改搜索架构, 则将需要请求爬网和重新建立索引。 按照对[网站、库或列表的手动请求爬网和重新编制索引](https://docs.microsoft.com/sharepoint/crawl-site-content)中的步骤, 对内容进行**重新编制索引**。 这可能需要一段时间, 等待24小时后再次检查结果。

有关详细信息, 请参阅[使网站上的内容](https://docs.microsoft.com/sharepoint/make-site-content-searchable)可供搜索。 
  
