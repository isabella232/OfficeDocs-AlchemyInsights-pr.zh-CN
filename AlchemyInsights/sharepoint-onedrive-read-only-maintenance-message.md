---
title: 在尝试使用 SharePoint 或 OneDrive 时, 维护邮件为只读
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 5b1e56253d6deeb0f9ba2f753eff5c00ff9c51a2
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620713"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="5bc47-102">在尝试使用 SharePoint 或 OneDrive 时, 维护邮件为只读</span><span class="sxs-lookup"><span data-stu-id="5bc47-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="5bc47-103">当尝试将 SharePoint 或 OneDrive 用于下列方案之一时, 用户可能会收到**只读的维护**消息。</span><span class="sxs-lookup"><span data-stu-id="5bc47-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="5bc47-104">计划的或活动的维护活动。</span><span class="sxs-lookup"><span data-stu-id="5bc47-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="5bc47-105">通过导航到[邮件中心](https://portal.office.com/adminportal/home#/messagecenter)来检查它们。</span><span class="sxs-lookup"><span data-stu-id="5bc47-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="5bc47-106">可能发生的高优先级活动服务事件。</span><span class="sxs-lookup"><span data-stu-id="5bc47-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="5bc47-107">通过导航到 "[服务运行状况](https://portal.office.com/adminportal/home#/servicehealth)" 检查是否有任何咨询/事件。</span><span class="sxs-lookup"><span data-stu-id="5bc47-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="5bc47-108">一种很小的自动修复恢复方案, 由于可能持续30分钟以上的服务器上的任何意外事件而发生。</span><span class="sxs-lookup"><span data-stu-id="5bc47-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="5bc47-109">这些次要恢复没有邮件中心或服务运行状况帖子, 但您应尽快恢复正常。</span><span class="sxs-lookup"><span data-stu-id="5bc47-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="5bc47-110">在极少数情况下, 我们发现上面列出的三个方案中的一种原因是原因, 服务已还原, 但尚未清除用户浏览器缓存。</span><span class="sxs-lookup"><span data-stu-id="5bc47-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="5bc47-111">请先尝试清除浏览器缓存, 然后再导航到该网站。</span><span class="sxs-lookup"><span data-stu-id="5bc47-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="5bc47-112">在 Microsoft Edge 浏览器中, 选择 "**设置**", 然后选择 "**隐私和安全**"。</span><span class="sxs-lookup"><span data-stu-id="5bc47-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="5bc47-113">在 "**清除浏览**" 下, 选择 "**选择要清除的内容**"。</span><span class="sxs-lookup"><span data-stu-id="5bc47-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="5bc47-114">选择 " **cookie" 和 "保存的网站数据**", 然后选择 "**清除**"。</span><span class="sxs-lookup"><span data-stu-id="5bc47-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="5bc47-115">这些步骤在使用其他浏览器 (如 Mozilla Firefox 或 Google Chrome) 时可能有所不同。</span><span class="sxs-lookup"><span data-stu-id="5bc47-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="5bc47-116">另一种方法是在新的 InPrivate 窗口中打开 SharePoint 网站或 OneDrive。</span><span class="sxs-lookup"><span data-stu-id="5bc47-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>