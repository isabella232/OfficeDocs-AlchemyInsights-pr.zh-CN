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
ms.openlocfilehash: 261fe1b1bc815dd4ad568051cfefad1e214b957e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530853"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="07fda-102">未向 SharePoint 列表或库发送工作流电子邮件</span><span class="sxs-lookup"><span data-stu-id="07fda-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="07fda-103">来自工作流的电子邮件不会发送给所有用户或仅发送给特定用户, 也不会看到错误**电子邮件无法发送。请确保电子邮件具有有效的收件人**。</span><span class="sxs-lookup"><span data-stu-id="07fda-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="07fda-104">检查用户是否存在于该网站集的 "**所有人员**权限" 组 ("用户信息" 列表中)。</span><span class="sxs-lookup"><span data-stu-id="07fda-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="07fda-105">示例直接 URL: https://<tenant>sharepoint.com/sites/<sitename>/_layouts/15/people.aspx？MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="07fda-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="07fda-106">如果用户不存在, 请确保用户已登录到页面。</span><span class="sxs-lookup"><span data-stu-id="07fda-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="07fda-107">如果是外部用户, 请确保已接受其邀请。</span><span class="sxs-lookup"><span data-stu-id="07fda-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="07fda-108">如果用户在权限组中确实存在, 请确保电子邮件地址正确无误。</span><span class="sxs-lookup"><span data-stu-id="07fda-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="07fda-109">如果未在此处设置用户电子邮件地址, 则为该用户创建一个示例通知, 以强制将该用户帐户从 SharePoint 的用户配置文件同步到此网站集。</span><span class="sxs-lookup"><span data-stu-id="07fda-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="07fda-110">来自工作流的电子邮件将发送给网站集管理员, 但不发送给其他用户, 并查看错误**HTTP 禁止访问<span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**。</span><span class="sxs-lookup"><span data-stu-id="07fda-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="07fda-111">在向[SharePoint 组发送电子邮件时, 请参阅访问被拒绝](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)。</span><span class="sxs-lookup"><span data-stu-id="07fda-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="07fda-112">此外, 确认 "**受限访问用户权限锁定模式**" 网站集功能未处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="07fda-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="07fda-113">相关主题</span><span class="sxs-lookup"><span data-stu-id="07fda-113">Related topics</span></span>
<span data-ttu-id="07fda-114">想要在 SharePoint Online 中试用 Microsoft 流吗？</span><span class="sxs-lookup"><span data-stu-id="07fda-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="07fda-115">创建流</span><span class="sxs-lookup"><span data-stu-id="07fda-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="07fda-116">SharePoint 和流</span><span class="sxs-lookup"><span data-stu-id="07fda-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


