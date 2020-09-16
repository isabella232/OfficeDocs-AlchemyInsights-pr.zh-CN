---
title: 删除 Teams 专用频道
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 56021a335c64810700913cf08519b95f24a7a17d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730905"
---
# <a name="delete-a-teams-private-channel"></a><span data-ttu-id="d5c4c-102">删除 Teams 专用频道</span><span class="sxs-lookup"><span data-stu-id="d5c4c-102">Delete a Teams private channel</span></span>

<span data-ttu-id="d5c4c-103">Microsoft 注意到，如果为基础 SharePoint 网站启用了 SharePoint 保留策略，则删除 Teams 专用频道时会遇到问题。</span><span class="sxs-lookup"><span data-stu-id="d5c4c-103">Microsoft is aware of an issue deleting a Teams private channel if you have SharePoint Retention Policies enabled for the underlying SharePoint site.</span></span> <span data-ttu-id="d5c4c-104">Microsoft 正在着手解决这一问题。</span><span class="sxs-lookup"><span data-stu-id="d5c4c-104">Microsoft is working on a fix.</span></span> <span data-ttu-id="d5c4c-105">在此期间，可以使用以下解决方法删除专用频道。</span><span class="sxs-lookup"><span data-stu-id="d5c4c-105">In the meantime, you can use the following workarounds to delete the private channel.</span></span>

<span data-ttu-id="d5c4c-106">**从 Sharepoint 保留策略中排除团队/网站集。**</span><span class="sxs-lookup"><span data-stu-id="d5c4c-106">**Exclude the Team/site collection from the Sharepoint retention policy.**</span></span>

1. <span data-ttu-id="d5c4c-107">转到 Office 365 管理门户，然后在左侧导航窗格中选择“**全部显示**”。</span><span class="sxs-lookup"><span data-stu-id="d5c4c-107">Go to the Office 365 admin portal, and select **Show all** in the left navigation pane.</span></span>
2. <span data-ttu-id="d5c4c-108">在**管理中心**下，转到“**安全与合规**” > “**数据丢失防护**” > “**策略**”。</span><span class="sxs-lookup"><span data-stu-id="d5c4c-108">Under **Admin centers**, go to **Security & Compliance** > **Data Loss Prevention** > **Policy**.</span></span>
3. <span data-ttu-id="d5c4c-109">确定适用于 SharePoint 网站的任何策略，并修改策略，以便包含专用频道的团队的 SharePoint 网站不包含在保留策略中。</span><span class="sxs-lookup"><span data-stu-id="d5c4c-109">Identify any policy that applies to Sharepoint sites, and modify the policy so the Sharepoint site for the Team containing the private channel is NOT included under the retention policy.</span></span>
4. <span data-ttu-id="d5c4c-110">保存策略。</span><span class="sxs-lookup"><span data-stu-id="d5c4c-110">Save the policy.</span></span>
    <span data-ttu-id="d5c4c-111">策略设置可能需要长达 24 小时才能生效。</span><span class="sxs-lookup"><span data-stu-id="d5c4c-111">It can take up to 24 hours for policy settings to take effect.</span></span>
    <span data-ttu-id="d5c4c-112">排除网站后，可删除专用频道。</span><span class="sxs-lookup"><span data-stu-id="d5c4c-112">After the site has been excluded, you can delete the private channel.</span></span>  
    
<span data-ttu-id="d5c4c-113">你***也许***能够通过在 Android 设备上使用 Microsoft Teams 删除专用频道。</span><span class="sxs-lookup"><span data-stu-id="d5c4c-113">You  ***might*** be able to delete the private channel by using Microsoft Teams on your Android device.</span></span> 

<span data-ttu-id="d5c4c-114">有关 SharePoint 的相关信息，请参阅[无法删除 SharePoint Online 或 OneDrive for Business 中的项目](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold)。</span><span class="sxs-lookup"><span data-stu-id="d5c4c-114">For related SharePoint information, see [Unable to delete items in SharePoint Online or OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span></span>