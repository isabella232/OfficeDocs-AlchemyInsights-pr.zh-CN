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
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731553"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>超过每日电子邮件限制。 工作流已挂起。

在以下情况下，可能会收到此错误：

- 您在 SharePoint Online 中有一个使用 SharePoint 2010 或 SharePoint 2013 工作流平台类型的工作流。
- 将工作流配置为将自定义电子邮件一次发送给多于200个用户的用户、每天多于10000个收件人，或每分钟30封以上的邮件。
- 运行工作流时，不会发送电子邮件，您会注意到以下行为：
    - 对于使用 SharePoint 2013 平台类型的工作流，请浏览到 " **工作流状态** " 页。 在 "工作流状态" 页上，" **内部状态** " 设置为 " **已启动**"，并且信息气球显示 **无法发送给收件人**。

若要解决此问题，请将工作流配置为在不超过 [Exchange Online 发件人限制](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits)的情况下发送电子邮件。 例如，在工作流中使用暂停，将电子邮件发送到 Microsoft 365 组、通讯组或启用邮件的安全组，或一次将邮件发送给少于200个收件人。


有关详细信息，请参阅以下 [文章](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)。

## <a name="related-topics"></a>相关主题
- [创建流](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint 和流](https://flow.microsoft.com/blog/sharepoint-and-flow/) 