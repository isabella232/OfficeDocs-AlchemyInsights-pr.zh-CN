---
title: Microsoft 团队-来宾访问
ms.author: heidip
author: microsoftheidi
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "311"
- "6500001"
ms.openlocfilehash: da9ecca062bd5f1dcc169657483ba53eb201def0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47798366"
---
# <a name="microsoft-teams---guest-access"></a><span data-ttu-id="62d43-102">Microsoft 团队-来宾访问</span><span class="sxs-lookup"><span data-stu-id="62d43-102">Microsoft Teams - Guest Access</span></span>

<span data-ttu-id="62d43-103">如果您需要帮助与团队中的组织外部用户进行通信，则需要决定是使用 [来宾访问还是外部访问 (联合) ](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access)，也可以同时使用这两者。</span><span class="sxs-lookup"><span data-stu-id="62d43-103">If you need help communicating with users outside your Organization in Teams, you need to decide whether to use [Guest Access or External Access (Federation)](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access), or you can use both.</span></span>

<span data-ttu-id="62d43-104">请务必 [查看差异](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access) 以了解每个可用的功能。</span><span class="sxs-lookup"><span data-stu-id="62d43-104">Be sure to [review the differences](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access) to understand the features available for each.</span></span>  <span data-ttu-id="62d43-105">例如，外部访问 (联合) 允许1:1 通信，如聊天和状态。</span><span class="sxs-lookup"><span data-stu-id="62d43-105">For example, External access (federation) allows for 1:1 communications, like Chat and Presence.</span></span>  <span data-ttu-id="62d43-106">但是，联合用户不能参与工作组协作。</span><span class="sxs-lookup"><span data-stu-id="62d43-106">Federated users cannot participate in Teams collaboration however.</span></span>  <span data-ttu-id="62d43-107">如果你想要外部用户加入团队频道对话或共享文件，你将需要启用来宾访问。</span><span class="sxs-lookup"><span data-stu-id="62d43-107">If you’d like an external user to join and participate in Teams Channel Conversations or Share Files, you’ll need to turn on Guest Access.</span></span>

<span data-ttu-id="62d43-108">**选项1：启用来宾访问** </span><span class="sxs-lookup"><span data-stu-id="62d43-108">**Option 1: Turn on Guest Access** </span></span>  
<span data-ttu-id="62d43-109">在团队管理中心，转到 " [组织范围的设置" > 来宾访问](https://admin.teams.microsoft.com/company-wide-settings/guest-configuration) 并打开 "允许在团队来宾访问"。</span><span class="sxs-lookup"><span data-stu-id="62d43-109">In the Teams Admin Center, Go to [Org Wide Settings > Guest Access](https://admin.teams.microsoft.com/company-wide-settings/guest-configuration) and turn on “Allow Guest Access in Teams”.</span></span>  <span data-ttu-id="62d43-110">对于具有所有其他默认设置的租户，您需要执行的所有操作。</span><span class="sxs-lookup"><span data-stu-id="62d43-110">For a tenant with all other default settings, this should be all you need to do.</span></span>  <span data-ttu-id="62d43-111">若要自定义来宾访问配置，请确保执行 [来宾访问检查表](https://docs.microsoft.com/microsoftteams/guest-access-checklist)中的所有步骤。</span><span class="sxs-lookup"><span data-stu-id="62d43-111">To customize your Guest Access configuration,  make sure you follow all the steps in the [Guest Access Checklist](https://docs.microsoft.com/microsoftteams/guest-access-checklist).</span></span> <span data-ttu-id="62d43-112">完成后，你需要 [等待24小时](https://docs.microsoft.com/microsoftteams/manage-guests#guest-access-latencies) 才能使设置生效。</span><span class="sxs-lookup"><span data-stu-id="62d43-112">Once you're completely done, you'll need to [wait up to 24 hours](https://docs.microsoft.com/microsoftteams/manage-guests#guest-access-latencies) for the settings to take effect.</span></span>

<span data-ttu-id="62d43-113">如果你确信已完成检查表中的所有步骤，并且已超过24小时，请继续操作并尝试 [将来宾添加到你的团队](https://support.office.com/article/add-guests-to-a-team-in-teams-fccb4fa6-f864-4508-bdde-256e7384a14f#ID0EAABAAA=Desktop)。</span><span class="sxs-lookup"><span data-stu-id="62d43-113">If you’re confident you’ve completed all the steps in the Checklist, and it's been more than 24 hours, go ahead and try to [add a Guest to your Team](https://support.office.com/article/add-guests-to-a-team-in-teams-fccb4fa6-f864-4508-bdde-256e7384a14f#ID0EAABAAA=Desktop).</span></span>

<span data-ttu-id="62d43-114">有关详细信息（包括操作方法视频），请参阅 [Microsoft 团队中的来宾访问](https://docs.microsoft.com/microsoftteams/guest-access)。</span><span class="sxs-lookup"><span data-stu-id="62d43-114">For more information, including how-to videos, see [Guest access in Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access).</span></span>

<span data-ttu-id="62d43-115">\*\*选项2：打开外部访问 (联合) \*\* 如果你还想打开外部 Access (联合) ，请在 "团队管理中心" 中转到 " [组织范围的设置" > "外部访问](https://admin.teams.microsoft.com/company-wide-settings/external-communications) "，并打开 "用户可以与 Skype for Business 和团队用户通信"，然后按照中的所有步骤操作， [让你的团队用户与另一个组织中的用户聊天并与之通信](https://docs.microsoft.com/microsoftteams/manage-external-access#let-your-teams-users-chat-and-communicate-with-users-in-another-organization)。</span><span class="sxs-lookup"><span data-stu-id="62d43-115">**Option 2: Turn On External Access (Federation)** If you’d also like to turn on External Access (Federation), in the Teams Admin center go to [Org-wide Settings > External Access](https://admin.teams.microsoft.com/company-wide-settings/external-communications) and turn on "Users can communicate with Skype for Business and Teams users", and then follow all the steps in [Let your Teams users chat and communicate with users in another organization](https://docs.microsoft.com/microsoftteams/manage-external-access#let-your-teams-users-chat-and-communicate-with-users-in-another-organization).</span></span>


