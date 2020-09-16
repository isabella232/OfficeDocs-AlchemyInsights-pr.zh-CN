---
title: Teams 允许或禁用 IP 视频
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002537"
- "5617"
ms.openlocfilehash: cf2d67170f846db1d5d2f1ca8c8b50902e200e45
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670174"
---
# <a name="teams-allow-or-disable-ip-video"></a><span data-ttu-id="ce280-102">Teams 允许或禁用 IP 视频</span><span class="sxs-lookup"><span data-stu-id="ce280-102">Teams allow or disable IP video</span></span>

<span data-ttu-id="ce280-103">**更改或创建会议策略**</span><span class="sxs-lookup"><span data-stu-id="ce280-103">**Change or create a meeting policy**</span></span>

<span data-ttu-id="ce280-104">若要更改或创建会议策略，请转到 **Microsoft Teams 管理中心 > 会议 > 会议策略**。</span><span class="sxs-lookup"><span data-stu-id="ce280-104">To change or create a meeting policy, go to the **Microsoft Teams admin center > Meetings > Meeting policies**.</span></span> <span data-ttu-id="ce280-105">从列表中选择一个策略，或者单击“**添加**”。</span><span class="sxs-lookup"><span data-stu-id="ce280-105">Select a policy from the list or click **Add**.</span></span> <span data-ttu-id="ce280-106">如果正在创建新策略，则添加名称和说明。</span><span class="sxs-lookup"><span data-stu-id="ce280-106">If you're creating a new policy, add a name and description.</span></span> <span data-ttu-id="ce280-107">名称不能包含特殊字符或超过 64 个字符。</span><span class="sxs-lookup"><span data-stu-id="ce280-107">The name can't contain special characters or be longer than 64 characters.</span></span> <span data-ttu-id="ce280-108">选择设置，然后单击“保存”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="ce280-108">Choose your settings, and then click **Save**.</span></span>

<span data-ttu-id="ce280-109">例如，假设你有很多用户并且你想要限制这些用户的会议所需的带宽量。</span><span class="sxs-lookup"><span data-stu-id="ce280-109">For example, say you have many users and you want to limit the amount of bandwidth that their meeting would require.</span></span> <span data-ttu-id="ce280-110">你要创建新的自定义策略并命名为“带宽限制”，然后禁用以下设置：</span><span class="sxs-lookup"><span data-stu-id="ce280-110">You would create a new custom policy named "Limited bandwidth" and disable the following settings:</span></span>

<span data-ttu-id="ce280-111">在“音频和视频”中：\*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="ce280-111">Under **Audio & video**:</span></span>

- <span data-ttu-id="ce280-112">禁用“允许云录制”。</span><span class="sxs-lookup"><span data-stu-id="ce280-112">Turn off Allow cloud recording.</span></span>
- <span data-ttu-id="ce280-113">禁用“允许 IP 视频”。</span><span class="sxs-lookup"><span data-stu-id="ce280-113">Turn off Allow IP video.</span></span>

<span data-ttu-id="ce280-114">然后将此策略分配给用户。</span><span class="sxs-lookup"><span data-stu-id="ce280-114">Then assign the policy to the users.</span></span>

<span data-ttu-id="ce280-115">**将会议策略分配给用户**</span><span class="sxs-lookup"><span data-stu-id="ce280-115">**Assign a meeting policy to users**</span></span>

1. <span data-ttu-id="ce280-116">在 Microsoft Teams 管理员中心的左侧导航中，转到“用户”，然后单击相应的用户。\*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="ce280-116">In the left navigation of the Microsoft Teams admin center, go to **Users**, and then click the user.</span></span>
2. <span data-ttu-id="ce280-117">单击用户名的左侧以选择用户，然后单击“编辑设置”。\*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="ce280-117">Select the user by clicking to the left of the user name, and then click **Edit settings**.</span></span>
3. <span data-ttu-id="ce280-118">在 **“会议策略”** 中，选择想要分配的策略，然后单击 **“应用”**。</span><span class="sxs-lookup"><span data-stu-id="ce280-118">Under **Meeting policy**, select the policy you want to assign and then click **Apply**.</span></span>

<span data-ttu-id="ce280-119">若要了解详细信息，请参阅[管理 Teams 中的会议策略](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)。</span><span class="sxs-lookup"><span data-stu-id="ce280-119">For more information, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>
