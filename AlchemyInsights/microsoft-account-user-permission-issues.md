---
title: 问题疑难解答-在目录中找不到用户
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 81b9dafe8e27e5f73fe232c51ff56fed3fec29b4
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36754182"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="10205-102">问题疑难解答-在目录中找不到用户</span><span class="sxs-lookup"><span data-stu-id="10205-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="10205-103">如果用户在目录中收到错误消息 "找不到用户"。</span><span class="sxs-lookup"><span data-stu-id="10205-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="10205-104">请重试问题类型为 "用户不在目录中" 的。</span><span class="sxs-lookup"><span data-stu-id="10205-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="10205-105">若要解决问题，可以完成以下步骤。</span><span class="sxs-lookup"><span data-stu-id="10205-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="10205-106">确保接受电子邮件邀请的帐户是以后用于登录的帐户。</span><span class="sxs-lookup"><span data-stu-id="10205-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="10205-107">请确保用户使用相同的帐户接受邀请并登录网站。</span><span class="sxs-lookup"><span data-stu-id="10205-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="10205-108">有关详细信息，请参阅[如何管理你的 Microsoft 帐户</a>的别名以管理 Office 365 登录名](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases)。</span><span class="sxs-lookup"><span data-stu-id="10205-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="10205-109">浏览到用户收到错误的每个站点。</span><span class="sxs-lookup"><span data-stu-id="10205-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="10205-110">将 "/_layouts/15/people.aspx/membershipgroupid = 0" （在双引号内）添加到网站 URL 的末尾。</span><span class="sxs-lookup"><span data-stu-id="10205-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="10205-111">示例： https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0。</span><span class="sxs-lookup"><span data-stu-id="10205-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="10205-112">从列表中选择用户。</span><span class="sxs-lookup"><span data-stu-id="10205-112">Select the user from the list.</span></span>

- <span data-ttu-id="10205-113">单击功能区中的 "**删除用户权限**"。</span><span class="sxs-lookup"><span data-stu-id="10205-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="10205-114">重新添加用户并将邀请重新发送给用户。</span><span class="sxs-lookup"><span data-stu-id="10205-114">Add back the User and Resend the invite to the user.</span></span>

