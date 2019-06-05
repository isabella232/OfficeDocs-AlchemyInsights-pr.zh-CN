---
title: 创建和使用共享邮箱
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 1825cfd0a78a29734d0a5128e19acbfba9115d32
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2019
ms.locfileid: "34717337"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="bc3c2-102">问题疑难解答-在目录中找不到用户</span><span class="sxs-lookup"><span data-stu-id="bc3c2-102">Troubleshoot issue - User not found in directory</span></span>

<p><span data-ttu-id="bc3c2-103">如果用户收到错误消息<strong> &ldquo; &hellip;, 则无法&rsquo;在目录中找到用户。请稍后重&hellip;试</strong>问题类型为<strong> &ldquo;"用户不在目录中&rdquo;</strong>" 的。, 可以完成以下步骤以解决问题。</span><span class="sxs-lookup"><span data-stu-id="bc3c2-103">If users are receiving error message <strong>&ldquo;&hellip;user can&rsquo;t be found in the directory. Please try again&hellip;&rdquo;</strong> where the Issue Type is <strong>&ldquo;User not in directory.&rdquo;</strong>, the following steps can be completed to troubleshoot the issue.</span></span></p> <ol> <li><span data-ttu-id="bc3c2-104">确保接受电子邮件邀请的帐户是以后用于登录的帐户。</span><span class="sxs-lookup"><span data-stu-id="bc3c2-104">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="bc3c2-105">请确保用户使用相同的帐户接受邀请并登录网站。</span><span class="sxs-lookup"><span data-stu-id="bc3c2-105">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> <br /><br /><span data-ttu-id="bc3c2-106">有关详细信息, 请参阅<a href="https://support.microsoft.com/en-us/help/12407/microsoft-account-how-to-manage-aliases">如何管理你的 Microsoft 帐户的别名</a>以管理 Office 365 登录名。</span><span class="sxs-lookup"><span data-stu-id="bc3c2-106">For more info, see <a href="https://support.microsoft.com/en-us/help/12407/microsoft-account-how-to-manage-aliases">How to manage aliases for your Microsoft account</a> to manage the Office 365 login.</span></span> <br /><br /></li> <li><span data-ttu-id="bc3c2-107">浏览到用户收到错误的每个站点。</span><span class="sxs-lookup"><span data-stu-id="bc3c2-107">Browse to each site(s) in which the user is receiving the error.</span></span> <br /><br /><span data-ttu-id="bc3c2-108">a.</span><span class="sxs-lookup"><span data-stu-id="bc3c2-108">a.</span></span> <span data-ttu-id="bc3c2-109">将<strong> &ldquo;/_layouts/15/people.aspx/membershipgroupid = 0&rdquo; </strong> (在双引号内) 添加到网站 URL 的末尾。</span><span class="sxs-lookup"><span data-stu-id="bc3c2-109">Add <strong>&ldquo;/_layouts/15/people.aspx/membershipgroupid=0&rdquo;</strong> (within the double-quotes) to the end of the site URL.</span></span> <br /><br /><span data-ttu-id="bc3c2-110">示例: https://&lt;contoso&gt;. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0</span><span class="sxs-lookup"><span data-stu-id="bc3c2-110">Example: https://&lt;contoso&gt;.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0</span></span> <br /><br /><span data-ttu-id="bc3c2-111">b.</span><span class="sxs-lookup"><span data-stu-id="bc3c2-111">b.</span></span> <span data-ttu-id="bc3c2-112">从列表中选择用户。</span><span class="sxs-lookup"><span data-stu-id="bc3c2-112">Select the user from the list.</span></span> <br /><br /><span data-ttu-id="bc3c2-113">c.</span><span class="sxs-lookup"><span data-stu-id="bc3c2-113">c.</span></span> <span data-ttu-id="bc3c2-114">单击<strong>功能区中的 "删除用户权限"</strong>。</span><span class="sxs-lookup"><span data-stu-id="bc3c2-114">Click <strong>Remove User Permissions from the Ribbon</strong>.</span></span> <br /><br /><span data-ttu-id="bc3c2-115">d.</span><span class="sxs-lookup"><span data-stu-id="bc3c2-115">d.</span></span> <span data-ttu-id="bc3c2-116">重新添加用户并将邀请重新发送给用户。</span><span class="sxs-lookup"><span data-stu-id="bc3c2-116">Add back the User and Resend the invite to the user.</span></span></li> </ol>

