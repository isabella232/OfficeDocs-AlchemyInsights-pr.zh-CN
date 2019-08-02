---
title: 未发送工作流电子邮件
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
- "1586"
ms.openlocfilehash: 783bf0a5721aa5db7088432c71e06cac6dc90513
ms.sourcegitcommit: 407f6c1e82f1a0be5cf53301fbf03cd25dcbf0ee
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/02/2019
ms.locfileid: "36059594"
---
# <a name="workflow-email-is-not-being-sent"></a><span data-ttu-id="ba4a0-102">未发送工作流电子邮件</span><span class="sxs-lookup"><span data-stu-id="ba4a0-102">Workflow email is not being sent</span></span>

1. <span data-ttu-id="ba4a0-103">来自工作流的电子邮件不会发送给所有用户或仅发送给特定用户, 也不会看到错误**电子邮件无法发送。请确保电子邮件具有有效的收件人**。</span><span class="sxs-lookup"><span data-stu-id="ba4a0-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

<span data-ttu-id="ba4a0-104">检查用户是否存在于该网站集的 "**所有人员**权限" 组 ("用户信息" 列表中)。</span><span class="sxs-lookup"><span data-stu-id="ba4a0-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="ba4a0-105">示例直接 URL: https://<tenant>sharepoint.com/sites/<sitename>/_layouts/15/people.aspx？MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="ba4a0-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

- <span data-ttu-id="ba4a0-106">如果用户不存在, 请确保用户已登录到页面。</span><span class="sxs-lookup"><span data-stu-id="ba4a0-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
- <span data-ttu-id="ba4a0-107">如果是外部用户, 请确保已接受其邀请。</span><span class="sxs-lookup"><span data-stu-id="ba4a0-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
- <span data-ttu-id="ba4a0-108">如果用户在权限组中确实存在, 请确保电子邮件地址正确无误。</span><span class="sxs-lookup"><span data-stu-id="ba4a0-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
- <span data-ttu-id="ba4a0-109">如果未在此处设置用户电子邮件地址, 则为该用户创建一个示例通知, 以强制将该用户帐户从 SharePoint 的用户配置文件同步到此网站集。</span><span class="sxs-lookup"><span data-stu-id="ba4a0-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="ba4a0-110">来自工作流的电子邮件将发送给网站集管理员, 而不是发送给其他用户, 并查看错误\*\*HTTP 禁止访问<spam> <spam>。 \*\* <spam> <spam></span><span class="sxs-lookup"><span data-stu-id="ba4a0-110">Email from Workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <spam><spam>https://URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**<spam><spam>.</span></span>
 

<span data-ttu-id="ba4a0-111">请参阅向[组发送电子邮件时访问被拒绝](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups)。</span><span class="sxs-lookup"><span data-stu-id="ba4a0-111">See [Access Denied when sent email to groups](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).</span></span>

<span data-ttu-id="ba4a0-112">此外, 确认 "**受限访问用户权限锁定模式**" 网站集功能未处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="ba4a0-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>

## <a name="related-topics"></a><span data-ttu-id="ba4a0-113">相关主题</span><span class="sxs-lookup"><span data-stu-id="ba4a0-113">Related topics</span></span>
- [<span data-ttu-id="ba4a0-114">创建流</span><span class="sxs-lookup"><span data-stu-id="ba4a0-114">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="ba4a0-115">SharePoint 和流</span><span class="sxs-lookup"><span data-stu-id="ba4a0-115">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


