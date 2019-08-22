---
title: SharePoint Online 中的搜索
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 3c3f6384172b2b4d59db6059618572db11059228
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507621"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a>SharePoint Online 中的内容爬网和索引

必须对内容进行爬网并将其添加到搜索索引中, 以便用户能够在 SharePoint Online 中查找他们搜索的内容。 根据预定义的爬网计划自动对内容进行爬网 (无法更改爬网计划)。 爬网程序选取自上次爬网以来已更改的内容，并更新索引。 若要确保对内容进行爬网并更新索引, 请注意以下事项:

- 确保可[搜索网站内容](https://docs.microsoft.com/sharepoint/make-site-content-searchable), 从而找到内容。

- 更改托管属性或更改已爬网和托管属性的映射后, 必须重新对网站进行爬网, 然后才能在搜索索引中反映您所做的更改。 

    由于您所做的更改是在搜索架构中进行的, 而不是实际网站, 因此爬网程序将不会自动对网站重新编制索引。 

    有关详细信息, 请参阅[手动对网站、库或列表的请求爬网和重新编制索引](https://docs.microsoft.com/sharepoint/crawl-site-conten)。

- 在手动请求爬网和完全重新索引以查看是否仍遇到问题后, 请至少等待24小时。 

    如果在你启动爬网和完全重新索引后超过了24小时, 请记录一个支持案例。 在许多情况下, 我们已经在努力解决了解决方案。 请至少为我们提供24小时的时间来完成解决方案。

> [!IMPORTANT]
> 如果网站、文档 (库) 或列表已删除且仍显示在搜索结果中, 则用户在尝试访问它时, 将收到**错误404文件 "找不**到"。 应将此问题作为进一步调查的支持案例进行记录。 



