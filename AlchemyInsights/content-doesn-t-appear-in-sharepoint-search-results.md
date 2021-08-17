---
title: 内容不会显示在SharePoint中
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: ca03c31def64e43935d734a17735b10373e5ca85b5f4ea0f0e886b9ea39884cd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54081600"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>内容不会显示在SharePoint中

当预期内容未显示在搜索结果中时，请按照以下疑难解答步骤操作：
  
1. 检查包含 **预期** 内容的网站是否设置为允许内容显示在搜索结果中。 按照在搜索结果中 [显示网站上的内容中的步骤操作](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results)。

2. 检查包含 **预期****内容的列表** 或库是否设置为允许内容显示在搜索结果中。 按照在搜索结果中 [显示列表或库中的内容中的步骤操作](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results)。

3. 验证页面、文档或自定义页面布局是否发布为主要 **版本。** 按照"搜索"中的步骤 3[操作，不会在 SharePoint Online 中返回所有结果](https://go.microsoft.com/fwlink/?linkid=874525)。

4. 验证用户是否 **有权** 查看内容。 按照了解中[的权限级别中的SharePoint。](https://docs.microsoft.com/sharepoint/understanding-permission-levels)
    
5. 如果通过添加新托管属性、编辑托管属性或删除托管属性更改了搜索架构，则请求爬网和重新编制索引是必需的。 **按照手动请求** 对网站、库或列表进行爬网和重新编制索引中的步骤，对内容 [重新编制索引](https://docs.microsoft.com/sharepoint/crawl-site-content)。 这可能需要一段时间，请等待 24 小时，然后再次检查结果。

有关详细信息，请参阅启用 [网站上的内容可搜索](https://docs.microsoft.com/sharepoint/make-site-content-searchable)。 
  
