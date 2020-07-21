---
title: SharePoint 中的 Yammer Web 部件
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5475"
- "9002494"
ms.openlocfilehash: 6868d7cdbbcc7d73e7e65fa0b0c954b4cba619ff
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2020
ms.locfileid: "45157275"
---
# <a name="yammer-web-parts-in-sharepoint"></a>SharePoint 中的 Yammer Web 部件

Yammer 对话和 Yammer Highlights web 部件，增强了对新式和经典 SharePoint 页面的协作性。 有关详细信息，请参阅[Yammer 对话](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#conversations)和[Yammer Highlights](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#highlights)。    

目前的 Yammer 对话 web 部件更新到了新的 Yammer 体验，可用于目标发布租户。 GA 推出已开始。 新增功能包括开始与任何帖子（提问、投票、表扬）的对话，以及标记直接从 SharePoint 获得最佳答案的功能。 有关更多信息，请参阅[新的 Yammer 客户条款和常见问题解答](https://docs.microsoft.com/yammer/get-started-with-yammer/newyammer-faq)。

 若要了解适合您的 Web 部件和配置，请参阅[在 SharePoint Online 中使用 Yammer Web 部件](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da)。  

**将 web 部件与 SharePoint Server 配合使用**  

Web 部件可以在本地环境中的新式和经典页面中使用。

- 有关新式页面的更多信息，请参阅[将 Yammer 源添加到 SharePoint Server 2019 的新式页面中](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-modern-page-in-sharepoint-server-2019)。 
- 有关经典页面的更多信息，请参阅[将 Yammer 源添加到 SharePoint Server 2013、2016 和 2019 的经典页面中](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-classic-page-in-sharepoint-servers-2013-2016-and-2019)。

**Yammer Embed**  

使用 Embed 配置工具来测试嵌入使用情况。 Embed 的将来更新将启用新的 Yammer 体验。 有关更多信息，请参见[Yammer Embed 配置工具](https://aka.ms/YammerEmbedConfigureTool)。 为了更好地了解 Yammer Embed 组件，请参阅[Embed 源](https://aka.ms/YammerDevDocs)。

**已知问题和限制**

- 组 ID 无法从已更改的新 Yammer URL 获得。 切换回经典模式以从 URL 获取组 ID 或其他 ID。
- 不支持自定义（虚）域。
- Yammer Embed 尚未针对移动设备进行优化。 在 Yammer 对话 Web部件上使用新式页面以获得最佳体验。
- 自定义主题可能会影响Y ammer 对话 Web 部件的外观和可用性。 打开支持案例以报告问题。