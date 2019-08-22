---
title: SharePoint Online 入门
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: ae27a9fc342eb4fc4633ffd5518d63600b978db8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36503985"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="d6191-102">SharePoint 中的工作流</span><span class="sxs-lookup"><span data-stu-id="d6191-102">Workflows in SharePoint</span></span>

<span data-ttu-id="d6191-103">如果 SharePoint 工作流不发送电子邮件, 则您的组织可能遇到了 Exchange Online 发件人限制。</span><span class="sxs-lookup"><span data-stu-id="d6191-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="d6191-104">如果您具有下列项之一, 则可能会出现 "工作流已挂起" 错误消息:</span><span class="sxs-lookup"><span data-stu-id="d6191-104">'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="d6191-105">您在 SharePoint Online 中有一个使用 SharePoint 2010 或 SharePoint 2013 工作流平台类型的工作流。</span><span class="sxs-lookup"><span data-stu-id="d6191-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="d6191-106">将工作流配置为将自定义电子邮件一次发送给多于200个用户的用户、每天多于10000个收件人, 或每分钟30封以上的邮件。</span><span class="sxs-lookup"><span data-stu-id="d6191-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="d6191-107">运行工作流时, 不会发送该电子邮件, 您会看到错误消息, "内部状态" 设置为 "已挂起" 或 "无法发送给收件人"。</span><span class="sxs-lookup"><span data-stu-id="d6191-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="d6191-108">有关详细信息, 请参阅以下[文章](https://support.office.com/article/-daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or-unable-to-send-to-a-recipient-error-in-a-sharepoint-online-workflow-89d02169-5fa6-4259-affc-73edb6ca9fb6?ui=en-US&amp;rs=en-US&amp;ad=US)。</span><span class="sxs-lookup"><span data-stu-id="d6191-108">For more information, please refer to the following [article](https://support.office.com/article/-daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or-unable-to-send-to-a-recipient-error-in-a-sharepoint-online-workflow-89d02169-5fa6-4259-affc-73edb6ca9fb6?ui=en-US&amp;rs=en-US&amp;ad=US).</span></span>

