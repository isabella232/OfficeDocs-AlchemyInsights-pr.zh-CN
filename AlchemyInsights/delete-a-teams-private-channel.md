---
title: 删除 Teams 专用频道
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 2ee998f0c70973645c273a2a6609af2420a4f74b
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431359"
---
# <a name="delete-a-teams-private-channel"></a><span data-ttu-id="93c86-102">删除 Teams 专用频道</span><span class="sxs-lookup"><span data-stu-id="93c86-102">Delete a Teams private channel</span></span>

<span data-ttu-id="93c86-103">Microsoft 注意到，如果为基础 SharePoint 网站启用了 SharePoint 保留策略，则删除 Teams 专用频道时会遇到问题。</span><span class="sxs-lookup"><span data-stu-id="93c86-103">Microsoft is aware of an issue deleting a Teams private channel if you have SharePoint Retention Policies enabled for the underlying SharePoint site.</span></span> <span data-ttu-id="93c86-104">Microsoft 正在着手解决这一问题。</span><span class="sxs-lookup"><span data-stu-id="93c86-104">Microsoft is working on a fix.</span></span> <span data-ttu-id="93c86-105">在此期间，可以使用以下解决方法删除专用频道。</span><span class="sxs-lookup"><span data-stu-id="93c86-105">In the meantime, you can use the following workarounds to delete the private channel.</span></span>

<span data-ttu-id="93c86-106">**从 Sharepoint 保留策略中排除团队/网站集。**</span><span class="sxs-lookup"><span data-stu-id="93c86-106">**Exclude the Team/site collection from the Sharepoint retention policy.**</span></span>

1. <span data-ttu-id="93c86-107">转到 Office 365 管理门户，然后在左侧导航窗格中选择“**全部显示**”。</span><span class="sxs-lookup"><span data-stu-id="93c86-107">Go to the Office 365 admin portal, and select **Show all** in the left navigation pane.</span></span>
2. <span data-ttu-id="93c86-108">在**管理中心**下，转到“**安全与合规**” > “**数据丢失防护**” > “**策略**”。</span><span class="sxs-lookup"><span data-stu-id="93c86-108">Under **Admin centers**, go to **Security & Compliance** > **Data Loss Prevention** > **Policy**.</span></span>
3. <span data-ttu-id="93c86-109">确定适用于 SharePoint 网站的任何策略，并修改策略，以便包含专用频道的团队的 SharePoint 网站不包含在保留策略中。</span><span class="sxs-lookup"><span data-stu-id="93c86-109">Identify any policy that applies to Sharepoint sites, and modify the policy so the Sharepoint site for the Team containing the private channel is NOT included under the retention policy.</span></span>
4. <span data-ttu-id="93c86-110">保存策略。</span><span class="sxs-lookup"><span data-stu-id="93c86-110">Save the policy.</span></span>
    <span data-ttu-id="93c86-111">策略设置可能需要长达 24 小时才能生效。</span><span class="sxs-lookup"><span data-stu-id="93c86-111">It can take up to 24 hours for policy settings to take effect.</span></span>
    <span data-ttu-id="93c86-112">排除网站后，可删除专用频道。</span><span class="sxs-lookup"><span data-stu-id="93c86-112">After the site has been excluded, you can delete the private channel.</span></span>  
    
<span data-ttu-id="93c86-113">你***也许***能够通过在 Android 设备上使用 Microsoft Teams 删除专用频道。</span><span class="sxs-lookup"><span data-stu-id="93c86-113">You  ***might*** be able to delete the private channel by using Microsoft Teams on your Android device.</span></span> 

<span data-ttu-id="93c86-114">有关 SharePoint 的相关信息，请参阅[无法删除 SharePoint Online 或 OneDrive for Business 中的项目](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold)。</span><span class="sxs-lookup"><span data-stu-id="93c86-114">For related SharePoint information, see [Unable to delete items in SharePoint Online or OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span></span>