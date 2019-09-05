---
title: 工作流未启动
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 2d85dcf9111d48cb529c583c733823b404eb3188
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36738079"
---
# <a name="workflow-is-not-starting"></a>工作流未启动

- SharePoint 2010 和 SharePoint 2013 工作流未启动。

    - 如果工作流未启动，则可能存在临时服务问题，用户可能会遇到工作流进度间歇延迟的问题。 检查[服务运行状况仪表板](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth)以查看您的组织是否受到影响。

    - 如果在你首次看到此问题后过去已经超过24小时，请记录一个支持票证。 在许多情况下，我们已经在努力解决了解决方案。 请至少为我们提供24小时的时间来完成解决方案。

- SharePoint 2010 工作流在启动时延迟。

    - 如果在大型批处理中触发工作流，则会发生此情况。 （例如，如果一次添加了多个项目）。

    - 工作流设计为实时运行，因此延迟是设计行为。

   -  如果工作流是复杂的可扩展对象标记语言（XMOL），则编译可能会很慢。 请[查看本文。](https://support.microsoft.com//kb/3043697)

    - 应简化工作流或使用 Microsoft SharePoint 2013 工作流平台类型对其进行重新设计。

    - 如果您的工作流历史记录增长很大，您可能需要清除这些项或创建一个新的历史记录列表。

        详细信息：[清除工作流历史记录](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>相关主题
想要在 SharePoint Online 中试用 Microsoft 流吗？
- [创建流](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint 和流](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


