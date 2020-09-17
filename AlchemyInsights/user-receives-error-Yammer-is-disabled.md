---
title: 用户收到错误 AADSTS7000112 Yammer 被禁用
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: 3a3a1b531f3d775f7e5150ce86733a3012df8d0e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47796638"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a><span data-ttu-id="47840-102">用户收到错误 AADSTS7000112 Yammer 被禁用</span><span class="sxs-lookup"><span data-stu-id="47840-102">User receives error AADSTS7000112 Yammer is disabled</span></span>

<span data-ttu-id="47840-103">如果收到错误“ AADSTS7000112：应用程序'00000005-0000-0ff1-ce00-000000000000'（Yammer）被禁用”，则 Azure AD 中的服务主体存在问题。</span><span class="sxs-lookup"><span data-stu-id="47840-103">If you receive the error "AADSTS7000112: Application '00000005-0000-0ff1-ce00-000000000000'(Yammer) is disabled", a problem exists with the service principal within Azure AD.</span></span> <span data-ttu-id="47840-104">管理员可能已禁用服务主体，阻止访问 Yammer。</span><span class="sxs-lookup"><span data-stu-id="47840-104">An administrator might have disabled the service principal to block access to Yammer.</span></span>

<span data-ttu-id="47840-105">建议不要禁用服务主体，否则会导致其他问题。</span><span class="sxs-lookup"><span data-stu-id="47840-105">Disabling the service principal is not recommended and can cause additional issues.</span></span> <span data-ttu-id="47840-106">有关阻止用户访问 Yammer 的支持方法的详细信息，请参阅[关闭 Microsoft 365 用户访问 Yammer ](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access)。</span><span class="sxs-lookup"><span data-stu-id="47840-106">For more info about the supported approach to block user access to Yammer, see [Turn off Yammer access for Microsoft 365 users](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span></span>  

<span data-ttu-id="47840-107">若要在 Azure 门户中更正此问题，并将用户访问权限还原到 Yammer：</span><span class="sxs-lookup"><span data-stu-id="47840-107">To correct this issue in the Azure Portal and restore user access to Yammer:</span></span>

1.  <span data-ttu-id="47840-108">打开 “Azure Active Directory”页面，然后在左侧导航窗格的“**管理**”下选择“**企业应用程序**”。</span><span class="sxs-lookup"><span data-stu-id="47840-108">Open the Azure Active Directory page, and select **Enterprise applications** under **Manage** in the left navigation pane.</span></span>
3.  <span data-ttu-id="47840-109">在搜索框中键入 \*\*Office 365 Yammer \*\*，然后选择应用程序名称以打开设置。</span><span class="sxs-lookup"><span data-stu-id="47840-109">Type **Office 365 Yammer** in the search box, and select the application name to open settings.</span></span>
4.  <span data-ttu-id="47840-110">在左侧导航窗格的“**管理**”下选择“**属性**”。</span><span class="sxs-lookup"><span data-stu-id="47840-110">Select **Properties** under **Manage** in the left navigation pane.</span></span>
5.  <span data-ttu-id="47840-111">将“**是否已启用供用户登录的值？**”设置为“**是**”，然后选择“**保存**”。</span><span class="sxs-lookup"><span data-stu-id="47840-111">Set the value of **Enabled for users to sign-in?** to **Yes**, and then select **Save**.</span></span>
6.  <span data-ttu-id="47840-112">重新登录 Yammer。</span><span class="sxs-lookup"><span data-stu-id="47840-112">Sign in to Yammer again.</span></span> <span data-ttu-id="47840-113">您可能需要清除 cookie。</span><span class="sxs-lookup"><span data-stu-id="47840-113">You might need to clear cookies.</span></span>

<span data-ttu-id="47840-114">或者运行 PowerShell 命令来设定数值。</span><span class="sxs-lookup"><span data-stu-id="47840-114">Alternatively, run PowerShell commands to set the value.</span></span> <span data-ttu-id="47840-115">有关更多信息，请参阅“[单击 Office 365 中的 Yammer 磁贴时，出现“抱歉，我们无法登录”错误](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365)”。</span><span class="sxs-lookup"><span data-stu-id="47840-115">For more info, see ["Sorry, but we're having trouble signing you in" error when you click the Yammer tile in Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span></span> 