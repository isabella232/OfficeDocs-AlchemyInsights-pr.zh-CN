---
title: 开始使用 Teams 实时事件
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
- "9000208"
- "3436"
ms.openlocfilehash: 979555a6fba46437adaf7e8c201cb9d6c4a8e965
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677269"
---
# <a name="getting-started-with-teams-live-events"></a><span data-ttu-id="da8a1-102">开始使用 Teams 实时事件</span><span class="sxs-lookup"><span data-stu-id="da8a1-102">Getting started with Teams live events</span></span>

<span data-ttu-id="da8a1-103">Microsoft Teams 实时事件是 Teams 会议的扩展，使您能够安排和制作流入大型在线受众的事件。</span><span class="sxs-lookup"><span data-stu-id="da8a1-103">Microsoft Teams live events are an extension of Teams meetings that enable you to schedule and produce events that stream to large online audiences.</span></span>

<span data-ttu-id="da8a1-104">若要创建实时事件，需执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="da8a1-104">To create a live event, you will need the following:</span></span>

- <span data-ttu-id="da8a1-105">首先，请确认 Teams 实时事件[在你所在的国家和地区可用](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability)；有些国家/地区尚不支持实时事件。</span><span class="sxs-lookup"><span data-stu-id="da8a1-105">First, confirm that Teams Live Events are [available in your Country and Region](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability); Live Events are not yet supported in some countries.</span></span>  <span data-ttu-id="da8a1-106">如果已分配许可证并设置了策略，但仍无法创建 Teams 实时事件，则可能是因为实时事件在你所在的国家或地区尚不可用。</span><span class="sxs-lookup"><span data-stu-id="da8a1-106">If you’ve assigned licenses and set policies, but still cannot create a Teams Live Event, it is likely you are in a Country or Region where Live Events is not yet available.</span></span>

- <span data-ttu-id="da8a1-107">[Office 365 企业版 E1、E3 或 E5 许可证，或 Office 365 A3 或 A5 许可证](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses)。</span><span class="sxs-lookup"><span data-stu-id="da8a1-107">An [Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span></span> <span data-ttu-id="da8a1-108">**注意**：由于最近 Teams 使用量增加，当向用户分配 Teams 许可证时，可能需要大约 24 小时才能完全设置。</span><span class="sxs-lookup"><span data-stu-id="da8a1-108">**Note**: Due to a recent increase in Teams usage, when you assign a Teams license to a user, it may take around 24 hours before they'll be fully set up.</span></span> <span data-ttu-id="da8a1-109">在此之前，将无法为他们分配团队策略，并且可能无法访问某些团队功能，例如呼叫和音频会议。</span><span class="sxs-lookup"><span data-stu-id="da8a1-109">Until then, you won't be able to assign Teams policies to them, and they might not have access to some Teams features like calling and audio conferencing.</span></span>

- <span data-ttu-id="da8a1-110">[在 Microsoft Teams 管理中心中创建实时事件](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy)的权限。</span><span class="sxs-lookup"><span data-stu-id="da8a1-110">Permission to [create live events in Microsoft Teams admin center](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy).</span></span>

- <span data-ttu-id="da8a1-111">[在 Microsoft Teams 中创建实时事件](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events)的权限。（适用于使用外部广播应用程序或设备制作的事件）。</span><span class="sxs-lookup"><span data-stu-id="da8a1-111">Permission to [create live events in Microsoft Stream](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (for events produced using an external broadcasting app or device).</span></span>

- <span data-ttu-id="da8a1-112">组织中的正式团队成员身份（不能是来宾或来自其他组织）。</span><span class="sxs-lookup"><span data-stu-id="da8a1-112">Full team membership in the org (can't be a guest or from another org).</span></span>
<span data-ttu-id="da8a1-113">私人会议计划、屏幕共享、IP 会议共享、已在 Team 会议策略中打开。</span><span class="sxs-lookup"><span data-stu-id="da8a1-113">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

- <span data-ttu-id="da8a1-114">Teams 实时事件[最佳做法](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42)。</span><span class="sxs-lookup"><span data-stu-id="da8a1-114">[Best practices](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42) for Teams Live Events.</span></span>

<span data-ttu-id="da8a1-115">有关更多信息，请查看“[Microsoft Teams 实时事件入门](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a)”。</span><span class="sxs-lookup"><span data-stu-id="da8a1-115">For more information, please see [Get started with Microsoft Teams live events](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a).</span></span>