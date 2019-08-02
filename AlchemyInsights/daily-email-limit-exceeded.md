---
title: 超过每日电子邮件限制。 工作流已挂起。
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 802aba696da61be5f0a6c12072842cbc3cd96499
ms.sourcegitcommit: 407f6c1e82f1a0be5cf53301fbf03cd25dcbf0ee
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/02/2019
ms.locfileid: "36059629"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="47a5b-103">超过每日电子邮件限制。</span><span class="sxs-lookup"><span data-stu-id="47a5b-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="47a5b-104">工作流已挂起。</span><span class="sxs-lookup"><span data-stu-id="47a5b-104">Workflow is suspended.</span></span>

<span data-ttu-id="47a5b-105">在以下情况下, 可能会收到此错误:</span><span class="sxs-lookup"><span data-stu-id="47a5b-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="47a5b-106">您在 SharePoint Online 中有一个使用 SharePoint 2010 或 SharePoint 2013 工作流平台类型的工作流。</span><span class="sxs-lookup"><span data-stu-id="47a5b-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="47a5b-107">将工作流配置为将自定义电子邮件一次发送给多于200个用户的用户、每天多于10000个收件人, 或每分钟30封以上的邮件。</span><span class="sxs-lookup"><span data-stu-id="47a5b-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="47a5b-108">运行工作流时, 不会发送电子邮件, 您会注意到以下行为:</span><span class="sxs-lookup"><span data-stu-id="47a5b-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="47a5b-109">对于使用 SharePoint 2013 平台类型的工作流, 请浏览到 "**工作流状态**" 页。</span><span class="sxs-lookup"><span data-stu-id="47a5b-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="47a5b-110">在 "工作流状态" 页上, "**内部状态**" 设置为 "**已启动**", 并且信息气球显示**无法发送给收件人**。</span><span class="sxs-lookup"><span data-stu-id="47a5b-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="47a5b-111">若要解决此问题, 请将工作流配置为在不超过[Exchange Online 发件人限制](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits)的情况下发送电子邮件。</span><span class="sxs-lookup"><span data-stu-id="47a5b-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="47a5b-112">例如, 在工作流中使用暂停, 将电子邮件发送到 Office 365 组、通讯组或启用邮件的安全组, 或一次将邮件发送给少于200个收件人。</span><span class="sxs-lookup"><span data-stu-id="47a5b-112">For example, use a pause in the workflow, send the email to an Office 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="47a5b-113">有关详细信息, 请参阅以下[文章](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)。</span><span class="sxs-lookup"><span data-stu-id="47a5b-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="47a5b-114">相关主题</span><span class="sxs-lookup"><span data-stu-id="47a5b-114">Related topics</span></span>
- [<span data-ttu-id="47a5b-115">创建流</span><span class="sxs-lookup"><span data-stu-id="47a5b-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="47a5b-116">SharePoint 和流</span><span class="sxs-lookup"><span data-stu-id="47a5b-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 