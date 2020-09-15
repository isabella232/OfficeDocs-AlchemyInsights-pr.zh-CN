---
title: SharePoint Online 入门
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: bba89489cb75555e1f508224de223bee04e1d665
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700697"
---
# <a name="workflows-in-sharepoint"></a>SharePoint 中的工作流

如果 SharePoint 工作流不发送电子邮件，则您的组织可能遇到了 Exchange Online 发件人限制。

如果您具有下列项之一，则可能会出现 "工作流已挂起" 错误消息：

- 您在 SharePoint Online 中有一个使用 SharePoint 2010 或 SharePoint 2013 工作流平台类型的工作流。

- 将工作流配置为将自定义电子邮件一次发送给多于200个用户的用户、每天多于10000个收件人，或每分钟30封以上的邮件。

运行工作流时，不会发送该电子邮件，您会看到错误消息，"内部状态" 设置为 "已挂起" 或 "无法发送给收件人"。

有关详细信息，请参阅以下 [文章](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running)。

