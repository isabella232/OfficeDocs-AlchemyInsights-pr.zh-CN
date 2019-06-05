---
title: 在 SharePoint Online 中管理搜索词典
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 4b51c6d44940c1a65ecf93a149430f05882452ba
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2019
ms.locfileid: "34715342"
---
# <a name="search-in-sharepoint-online"></a>SharePoint Online 中的搜索

<p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin; color: black; background: white;">必须对内容进行爬网并将其添加到搜索索引中, 以便用户能够在 SharePoint Online 中查找他们搜索的内容。根据预定义的爬网计划自动对内容进行爬网 (无法更改爬网计划)。爬网程序将选取自上次爬网后已更改的内容, 并更新索引。</span> 若要确保对内容进行爬网并更新索引, 请执行以下步骤。</p> <ol style="margin-top: 0in;" start="1" type="1"> <li style="color: black; ; font-size: 11pt; font-style: normal; font-weight: 400; margin-left: 0in;"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin; background: white;">确保可搜索网站内容, 从而找到内容。 有关详细信息, 请参阅<a href="https://docs.microsoft.com/en-us/sharepoint/make-site-content-searchable">使网站上的内容</a>可供搜索。 <br /><br /></span></li> <li style="color: black; ; font-size: 11pt; font-style: normal; font-weight: 400; margin-left: 0in;"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin; background: white;"><span style="display: inline !important; float: none; background-color: #ffffff; color: #000000; font-family: Segoe UI,SegoeUI,Segoe WP,Helvetica Neue,Helvetica,Tahoma,Arial,sans-serif; font-size: 16px; font-style: normal; font-variant: normal; font-weight: 400; letter-spacing: normal; orphans: 2; text-align: left; text-decoration: none; text-indent: 0px; text-transform: none; -webkit-text-stroke-width: 0px; white-space: normal; word-spacing: 0px;">更改托管属性或更改已爬网和托管属性的映射后,<strong>必须重新对网站进行爬网</strong>, 然后才能在搜索索引中反映您所做的更改。<span style="display: inline !important; float: none; background-color: #ffffff; color: #000000; font-family: Segoe UI,SegoeUI,Segoe WP,Helvetica Neue,Helvetica,Tahoma,Arial,sans-serif; font-size: 16px; font-style: normal; font-variant: normal; font-weight: 400; letter-spacing: normal; orphans: 2; text-align: left; text-decoration: none; text-indent: 0px; text-transform: none; -webkit-text-stroke-width: 0px; white-space: normal; word-spacing: 0px;">由于您所做的更改是在搜索架构中进行的, 而不是实际网站, 因此爬网程序将不会自动对网站重新编制索引。</span> </span> </span><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin; color: windowtext;">有关详细信息, 请参阅<a href="https://docs.microsoft.com/en-us/sharepoint/crawl-site-content">手动对网站、库或列表的请求爬网和重新编制索引</a>。&nbsp;<br /><br /></span><strong style="mso-bidi-font-weight: normal;"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">注意:</span> </strong> <span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">在手动请求爬网和完全重新索引以查看是否仍遇到问题后, 请至少等待24小时。 <span style="color: black; background: white;">如果在你启动爬网和完全重新索引后超过了24小时, 请记录一个支持案例。 在许多情况下, 我们已经在努力解决了解决方案。 请至少为我们提供24小时的时间来完成解决方案。<br /><br /></span></span><strong style="mso-bidi-font-weight: normal;"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">重要说明:</span></strong><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">如果网站、文档 (库) 或列表已删除且仍显示在搜索结果中, 则用户在尝试访问时, 将收到错误404文件 "找不到"。应将此问题作为进一步调查的支持案例进行记录。</span></li> </ol>



