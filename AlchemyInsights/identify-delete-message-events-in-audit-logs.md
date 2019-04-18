---
title: 确定审核日志中的删除邮件事件
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1370
ms.assetid: ''
ms.openlocfilehash: 93f8a192af6e689e2b2d04013f35b8da2b69e607
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909061"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="0ae02-102">已删除电子邮件的审核日志</span><span class="sxs-lookup"><span data-stu-id="0ae02-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="0ae02-103">从2019年1月起, Microsoft 将默认启用邮箱审核日志记录。</span><span class="sxs-lookup"><span data-stu-id="0ae02-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="0ae02-104">否则, 若要查看特定用户的删除邮件事件, 需要手动启用审核的删除操作。</span><span class="sxs-lookup"><span data-stu-id="0ae02-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="0ae02-105">如果已为您的组织或特定用户启用邮箱审核日志记录, 请执行以下步骤。</span><span class="sxs-lookup"><span data-stu-id="0ae02-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="0ae02-106">登录到[Office 365 安全 & 合规中心](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="0ae02-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="0ae02-107">单击 "**搜索和调查**", 然后选择 "**审核日志搜索**"。</span><span class="sxs-lookup"><span data-stu-id="0ae02-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="0ae02-108">在 "**开始日期**" 和 "**结束日期**" 字段中选择日期范围。</span><span class="sxs-lookup"><span data-stu-id="0ae02-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="0ae02-109">指定要调查的用户的用户名 (删除这些项目的用户)。</span><span class="sxs-lookup"><span data-stu-id="0ae02-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="0ae02-110">在 "**活动**" 字段中, 选择 "**已删除邮件" 文件夹**, 并**将邮件移动到 "已删除**邮件" 文件夹。</span><span class="sxs-lookup"><span data-stu-id="0ae02-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="0ae02-111">单击"搜索"。</span><span class="sxs-lookup"><span data-stu-id="0ae02-111">Click **Search**.</span></span>

<span data-ttu-id="0ae02-112">在结果中, 选择一个审核记录。</span><span class="sxs-lookup"><span data-stu-id="0ae02-112">In the results, select an audit record.</span></span> <span data-ttu-id="0ae02-113">在 "详细信息" 浮出控件中, 单击 "**详细信息**"。</span><span class="sxs-lookup"><span data-stu-id="0ae02-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="0ae02-114">在 " **AffectedItems** " 字段中显示有关已删除项目的其他信息 (例如, 在删除项目时的主题行和位置)。</span><span class="sxs-lookup"><span data-stu-id="0ae02-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="0ae02-115">**ClientInfoString**属性将显示在 outlook、outlook 网页 (以前称为 Outlook web App) 或任何其他设备上是否发生了删除。</span><span class="sxs-lookup"><span data-stu-id="0ae02-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="0ae02-116">有关详细信息, 请参阅[确定为邮箱设置电子邮件转发](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items)。</span><span class="sxs-lookup"><span data-stu-id="0ae02-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="0ae02-117">**注意**: 不能使用 "审核日志" 功能检索已删除的项目。</span><span class="sxs-lookup"><span data-stu-id="0ae02-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="0ae02-118">若要在 web 上的 Outlook 中检索已删除的邮件, 请参阅[在 outlook web App 中恢复已删除的项目](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)。</span><span class="sxs-lookup"><span data-stu-id="0ae02-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
