---
title: 订阅访问
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/27/2020
ms.locfileid: "48773769"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a><span data-ttu-id="ce112-102">由于浏览器问题 (浏览器挂起、保持旋转、不会加载等等，因此无法登录 Azure ) </span><span class="sxs-lookup"><span data-stu-id="ce112-102">Unable to Sign-in Azure due to browser issues (Browser hangs, keeps spinning, does not load, etc.)</span></span>

<span data-ttu-id="ce112-103">中断可能会受到影响。</span><span class="sxs-lookup"><span data-stu-id="ce112-103">You might be impacted by an outage.</span></span> <span data-ttu-id="ce112-104">请查看是否存在正在进行的中断： [Azure 运行状况状态](https://status.azure.com/status/history/)。</span><span class="sxs-lookup"><span data-stu-id="ce112-104">Please check to see if there is an ongoing outage: [Azure Health Status](https://status.azure.com/status/history/).</span></span>

<span data-ttu-id="ce112-105">请注销所有活动的 Azure 会话。</span><span class="sxs-lookup"><span data-stu-id="ce112-105">Please log out of all the active Azure sessions.</span></span> <span data-ttu-id="ce112-106">启动 web 浏览器的私有或 incognito 模式。</span><span class="sxs-lookup"><span data-stu-id="ce112-106">Start a in-private or incognito mode of your web browser.</span></span>

<span data-ttu-id="ce112-107">您还可以尝试刷新浏览器，使用另一个浏览器，如果上面不起作用，则删除缓存 cookie。</span><span class="sxs-lookup"><span data-stu-id="ce112-107">You could also try to Refresh browser, use another browser, delete cache cookies if above doesn't work.</span></span>

<span data-ttu-id="ce112-108">了解详细信息： [解决登录问题](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span><span class="sxs-lookup"><span data-stu-id="ce112-108">Learn more: [Troubleshoot Sign-in Issues](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span></span>

<span data-ttu-id="ce112-109">**无法访问订阅**</span><span class="sxs-lookup"><span data-stu-id="ce112-109">**Unable to access subscriptions**</span></span>

<span data-ttu-id="ce112-110">在 [Azure 门户](https://portal.azure.com/)中，请确保从右上角的帐户中选择了正确的 Azure 目录。</span><span class="sxs-lookup"><span data-stu-id="ce112-110">In the [Azure portal](https://portal.azure.com/), make sure that the correct Azure directory is selected from the account at the top right.</span></span>

<span data-ttu-id="ce112-111">在 [Azure 帐户中心](https://account.windowsazure.com/Subscriptions)中，确保使用的帐户是帐户管理员。</span><span class="sxs-lookup"><span data-stu-id="ce112-111">In the [Azure Account center](https://account.windowsazure.com/Subscriptions), make sure if the account used is the account admin.</span></span>

<span data-ttu-id="ce112-112">了解详细信息： [排除未找到订阅的故障](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="ce112-112">Learn more: [Troubleshoot No Subscriptions found](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="ce112-113">**无法访问帐单历史记录**</span><span class="sxs-lookup"><span data-stu-id="ce112-113">**Unable to access billing history**</span></span>

<span data-ttu-id="ce112-114">帐户管理员需要确保以来宾用户身份在 Azure Active directory 中添加访问帐单信息的用户： [添加或删除新用户](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support)。</span><span class="sxs-lookup"><span data-stu-id="ce112-114">The account admin needs to make sure the user accessing the billing information is added in the Azure Active directory as a guest user: [Add or delete a new user](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="ce112-115">然后，需要向用户授予全局管理员角色：为 [用户分配角色](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support)。</span><span class="sxs-lookup"><span data-stu-id="ce112-115">The user then needs to be given a Global admin role: [Assign role to users](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="ce112-116">发布此内容时，可以使用 RBAC 策略对用户授予帐单访问权限： [授予对帐单的访问权限](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)。</span><span class="sxs-lookup"><span data-stu-id="ce112-116">Post this, the user can be given billing access using RBAC policies: [Grant access to billing](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="ce112-117">**建议的文档**</span><span class="sxs-lookup"><span data-stu-id="ce112-117">**Recommended Documents**</span></span>

-   [<span data-ttu-id="ce112-118">我无法登录以管理我的 Azure 订阅</span><span class="sxs-lookup"><span data-stu-id="ce112-118">I can't sign in to manage my Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)