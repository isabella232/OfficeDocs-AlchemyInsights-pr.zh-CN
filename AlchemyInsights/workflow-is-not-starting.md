---
title: 工作流未启动
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 77a3c022a9a3a82041b4a4a70c72c2e0940c0fba27f296f07881e3abebf1e464
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53907728"
---
# <a name="workflow-is-not-starting"></a>工作流未启动

- SharePoint 2010 和 SharePoint 2013 工作流未启动。

    - 如果工作流未启动，则可能会遇到临时服务问题，用户可能会遇到工作流进度的间歇性延迟。 检查 [服务运行状况仪表板](https://admin.microsoft.com/AdminPortal/Home/servicehealth) 以查看您的组织是否受到影响。

    - 如果自你第一次看到此问题以来超过 24 小时，请记录支持票证。 在许多情况下，我们已经在研究解决方案。 请给我们至少 24 小时才能完成解决方案。

- SharePoint延迟的 2010 工作流。

    - 如果以大批量方式触发工作流，则会出现此情况。  (，例如，当一次添加多个项目时) 。

    - 工作流不是设计为实时运行，因此延迟是按设计行为。

   -  如果工作流是 XMOL 中复杂的可扩展对象标记 (语言) ，则编译速度可能很慢。 查看 [本文](https://support.microsoft.com//kb/3043697) 。

    - 您应该使用 Microsoft SharePoint 2013 工作流平台类型来简化工作流或重新设计它。

    - 如果您的工作流历史记录已变得很大，您可能需要清除项目或创建新的历史记录列表。

        详细信息： [清除工作流历史记录](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>相关主题
想要尝试在 Microsoft Flow Online SharePoint？
- [创建Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint 和 Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
