---
title: 超过每日电子邮件限制。 工作流已挂起。
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 60ddbe68298e998a4e0b271a15209efc135c80638702c98dbcb3e0b2f1554860
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914641"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>超过每日电子邮件限制。 工作流已挂起。

以下情况下可能会收到此错误：

- 在 SharePoint Online 中，您可以使用 SharePoint 2010 或 SharePoint 2013 工作流平台类型。
- 工作流配置为一次向 200 多个用户发送自定义电子邮件、每天 10，000 多个收件人或每分钟 30 多封邮件。
- 运行工作流时，不会发送电子邮件，并且您注意到以下行为：
    - 对于使用 SharePoint 2013 平台类型的工作流，您可以浏览到"**工作流状态"** 页。 在"工作流状态"页上，"**内部** 状态"设置为"已启动"，信息气球将显示"无法 **发送给收件人"。**

若要解决此问题，请将工作流配置为发送电子邮件，而不超出发件人Exchange Online[限制](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits)。 例如，在工作流中暂停、将电子邮件发送到 Microsoft 365 组、通讯组或启用邮件的安全组，或者一次将邮件发送给少于 200 个收件人。


有关详细信息，请参阅以下 [文章](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)。

## <a name="related-topics"></a>相关主题
- [创建Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint 和 Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 