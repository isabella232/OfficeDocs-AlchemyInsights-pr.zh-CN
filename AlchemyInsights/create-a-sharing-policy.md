---
title: 创建共享策略，以允许你的用户与组织外部的人员共享其日历
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 016b915a9e8f7e32d5d393bc47347991866647c7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816262"
---
# <a name="create-a-sharing-policy-to-allow-your-users-to-share-their-calendar-with-people-outside-your-organization"></a><span data-ttu-id="c72fe-102">创建共享策略，以允许你的用户与组织外部的人员共享其日历</span><span class="sxs-lookup"><span data-stu-id="c72fe-102">Create a Sharing Policy to allow your users to share their calendar with people outside your organization</span></span>

1. <span data-ttu-id="c72fe-103">从 Microsoft 365 管理中心主控板中，转到“**管理员**” > “**Exchange**”。</span><span class="sxs-lookup"><span data-stu-id="c72fe-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="c72fe-104">转到“**组织**” > “**共享**”。</span><span class="sxs-lookup"><span data-stu-id="c72fe-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="c72fe-105">在列表视图中的“**单个共享**”下，单击“**新建**”。</span><span class="sxs-lookup"><span data-stu-id="c72fe-105">In the list view, under **Individual Sharing**, click **New** .</span></span>
4. <span data-ttu-id="c72fe-106">在“**新建共享策略**”中，在“**策略名称**”框中为共享策略键入一个友好名称。</span><span class="sxs-lookup"><span data-stu-id="c72fe-106">In **new sharing policy**, type a friendly name for the sharing policy in the **Policy name** box.</span></span>
5. <span data-ttu-id="c72fe-107">单击“**添加**”定义策略的共享规则。</span><span class="sxs-lookup"><span data-stu-id="c72fe-107">Click **Add**  to define the sharing rules for the policy.</span></span>
6. <span data-ttu-id="c72fe-108">在“共享规则”中，选择以下选项之一以指定要共享的域：</span><span class="sxs-lookup"><span data-stu-id="c72fe-108">In **sharing rule**, select one of the following options to specify the domains you want to share with:</span></span>
    - <span data-ttu-id="c72fe-109">**与所有域共享**</span><span class="sxs-lookup"><span data-stu-id="c72fe-109">**Sharing with all domains**</span></span>
    - <span data-ttu-id="c72fe-110">**与特定域共享**</span><span class="sxs-lookup"><span data-stu-id="c72fe-110">**Sharing with a specific domain**</span></span>
8. <span data-ttu-id="c72fe-p101">如果选择了“与特定域共享”，请键入要与其共享的域的名称。如果需要为此共享策略输入多个域，请保存第一个域的设置，然后编辑共享规则，以添加更多的域。</span><span class="sxs-lookup"><span data-stu-id="c72fe-p101">If you select **Sharing with a specific domain**, type the name of the domain you want to share with. If you need to enter more than one domain for this sharing policy, save the settings for the first domain, then edit the sharing rules to add more domains.</span></span>
9. <span data-ttu-id="c72fe-113">若要指定可共享的信息，请选中“共享日历文件夹”复选框，然后选择以下选项之一：</span><span class="sxs-lookup"><span data-stu-id="c72fe-113">To specify the information that can be shared, select the **Share your calendar folder** check box, and then select one of the following options:</span></span>
    - <span data-ttu-id="c72fe-114">**仅包含时间的日历忙/闲信息**</span><span class="sxs-lookup"><span data-stu-id="c72fe-114">**Calendar free/busy information with time only**</span></span>
    - <span data-ttu-id="c72fe-115">**包含时间、主题和位置的日历忙/闲信息**</span><span class="sxs-lookup"><span data-stu-id="c72fe-115">**Calendar free/busy information with time, subject, and location**</span></span>
    - <span data-ttu-id="c72fe-116">**所有日历约会信息，包括时间、主题、位置和标题**</span><span class="sxs-lookup"><span data-stu-id="c72fe-116">**All calendar appointment information, including time, subject, location and title**</span></span>
11. <span data-ttu-id="c72fe-117">单击“保存”设置共享策略的规则。</span><span class="sxs-lookup"><span data-stu-id="c72fe-117">Click **save** to set the rules for the sharing policy.</span></span>
12. <span data-ttu-id="c72fe-118">如果希望将该共享策略设置为你组织中所有用户的新默认共享策略，可选中“**将该策略作为我的默认共享策略**”复选框。</span><span class="sxs-lookup"><span data-stu-id="c72fe-118">If you want to set this sharing policy as the new default sharing policy for all users in your organization, select the **Make this policy my default sharing policy** check box.</span></span>
13. <span data-ttu-id="c72fe-119">单击“**保存**”创建共享策略。</span><span class="sxs-lookup"><span data-stu-id="c72fe-119">Click **save** to create the sharing policy.</span></span>  

<span data-ttu-id="c72fe-120">**如需全面了解本主题，请阅读：**</span><span class="sxs-lookup"><span data-stu-id="c72fe-120">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="c72fe-121">在 Exchange Online 中创建共享策略</span><span class="sxs-lookup"><span data-stu-id="c72fe-121">Create a sharing policy in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/create-a-sharing-policy)
- [<span data-ttu-id="c72fe-122">将共享策略应用于 Exchange Online 中的邮箱</span><span class="sxs-lookup"><span data-stu-id="c72fe-122">Apply a sharing policy to mailboxes in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy)
- [<span data-ttu-id="c72fe-123">修改、禁用或删除 Exchange Online 中的共享策略</span><span class="sxs-lookup"><span data-stu-id="c72fe-123">Modify, disable, or remove a sharing policy in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)