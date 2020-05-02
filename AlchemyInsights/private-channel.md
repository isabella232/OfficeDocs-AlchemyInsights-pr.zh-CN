---
title: 专用通道
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001223"
- "3205"
ms.openlocfilehash: be518df0d40123c1f0da6596bd6e2e91a0c2c8fa
ms.sourcegitcommit: 057d87c9d866fa1371d02350420d13774545c028
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/02/2020
ms.locfileid: "44005428"
---
# <a name="private-channels-in-microsoft-teams"></a><span data-ttu-id="bd389-102">Microsoft 团队中的专用通道</span><span class="sxs-lookup"><span data-stu-id="bd389-102">Private channels in Microsoft Teams</span></span>

<span data-ttu-id="bd389-103">专用频道是 Microsoft 团队中的一项新功能。</span><span class="sxs-lookup"><span data-stu-id="bd389-103">Private channels is a new feature in Microsoft Teams.</span></span> <span data-ttu-id="bd389-104">请注意，专用通道不能从标准通道进行转换，反之亦然。</span><span class="sxs-lookup"><span data-stu-id="bd389-104">Note that private channels cannot be converted from standard channels or vice versa.</span></span>

<span data-ttu-id="bd389-105">有关专用通道的详细信息，例如[专用通道创建和成员身份](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership)和[专用通道 SharePoint 网站](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites)的信息，请参阅[Microsoft 团队中的专用频道](https://docs.microsoft.com/MicrosoftTeams/private-channels)。</span><span class="sxs-lookup"><span data-stu-id="bd389-105">For details about private channels, such as information on [private channel creation and membership](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) and [private channel SharePoint sites](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), see [Private channels in Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span></span> 

<span data-ttu-id="bd389-106">**注意：** 由于尚不支持用于保留专用通道邮件的配置，因此启用了保留策略的租户在默认情况下不会启用专用通道。</span><span class="sxs-lookup"><span data-stu-id="bd389-106">**Note:** Because configuration for retention of private channel messages is not yet supported, tenants with retention policies enabled will not have private channels enabled by default.</span></span> <span data-ttu-id="bd389-107">可以在团队管理中心启用专用通道。</span><span class="sxs-lookup"><span data-stu-id="bd389-107">Private channels can be enabled in the Teams admin center.</span></span> <span data-ttu-id="bd389-108">此外，请注意，虽然不支持保留专用通道消息，但支持在专用通道中共享的文件的保留。</span><span class="sxs-lookup"><span data-stu-id="bd389-108">Also, note that while retention of private channel messages is not supported, retention of files shared in private channels is supported.</span></span>

<span data-ttu-id="bd389-109">**是否需要新的团队所有者？**</span><span class="sxs-lookup"><span data-stu-id="bd389-109">**Need a new team owner?**</span></span>

<span data-ttu-id="bd389-110">如果你的专用渠道所有者离开，你可以通过团队 Powershell 添加新的团队所有者。</span><span class="sxs-lookup"><span data-stu-id="bd389-110">If your private channel owner leaves, you can add a new team owner via Teams Powershell.</span></span>


- <span data-ttu-id="bd389-111">转到[此处](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6)安装团队 Powershell。</span><span class="sxs-lookup"><span data-stu-id="bd389-111">Go [here](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) to install Teams Powershell.</span></span>

<span data-ttu-id="bd389-112">下面是你将需要的 cmdlet：</span><span class="sxs-lookup"><span data-stu-id="bd389-112">Here is the cmdlet you will need:</span></span>

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

<span data-ttu-id="bd389-113">有关团队 Powershell 的详细信息，请参阅[团队 Powershell 概述](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)。</span><span class="sxs-lookup"><span data-stu-id="bd389-113">For more information on Teams Powershell, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span>
