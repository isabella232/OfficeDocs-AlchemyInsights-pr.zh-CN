---
title: 日历事件缺失或未更新
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10932"
- "9001435"
ms.openlocfilehash: b114411d6285a68a41bbcbf64151c212ee2cf661
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819977"
---
# <a name="calendar-events-missing-or-not-updating"></a><span data-ttu-id="b476b-102">日历事件缺失或未更新</span><span class="sxs-lookup"><span data-stu-id="b476b-102">Calendar Events missing or not updating</span></span>

<span data-ttu-id="b476b-103">如果日历事件缺失或未更新，请首先在 Outlook 中查看日历文件夹属性中的项目计数：</span><span class="sxs-lookup"><span data-stu-id="b476b-103">If calendar items are missing or not updating, start by looking at the item count in your Calendar folder properties in Outlook:</span></span> 

1. <span data-ttu-id="b476b-104">右键单击受影响的用户 **日历** 文件夹，然后选择“**属性**”。</span><span class="sxs-lookup"><span data-stu-id="b476b-104">Right-click on the affected user **Calendar** folder, and then select **Properties**.</span></span>

1. <span data-ttu-id="b476b-105">选择“**同步**”选项卡。</span><span class="sxs-lookup"><span data-stu-id="b476b-105">Select the **Synchronization** tab.</span></span>

<span data-ttu-id="b476b-106">如果服务器文件夹和脱机文件夹之间的项目计数不同：</span><span class="sxs-lookup"><span data-stu-id="b476b-106">If the item count is not the same between the Server folder and the Offline Folder:</span></span>

1.  <span data-ttu-id="b476b-107">突出显示 **日历** 文件夹。</span><span class="sxs-lookup"><span data-stu-id="b476b-107">Highlight the **Calendar** folder.</span></span>

1.  <span data-ttu-id="b476b-108">转到“**发送**”/“**接收**”选项卡，然后选择“**更新文件夹**”。</span><span class="sxs-lookup"><span data-stu-id="b476b-108">Go to the **Send**/**Receive** tab, and then select **Update Folder**.</span></span>

<span data-ttu-id="b476b-109">如果仍未更新日历或缺少事件，请从 [Microsoft 下载中心](https://www.microsoft.com/download/details.aspx?id=28786)下载 Outlook 日历检查工具。</span><span class="sxs-lookup"><span data-stu-id="b476b-109">If your calendar is still not updating or events are missing, download the Calendar Checking Tool for Outlook from the [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=28786).</span></span> <span data-ttu-id="b476b-110">确定日历文件夹中的项目是否超过 5000 个，因为这可能导致日历会议未更新或会议错误等现象。</span><span class="sxs-lookup"><span data-stu-id="b476b-110">Determine if there are more than 5000 items in the calendar folder as this can cause symptoms such as calendar meetings not updated or meeting errors.</span></span> 

<span data-ttu-id="b476b-111">有关详细信息，请参阅[缓存模式 .ost 或 .pst 文件中的项目或文件夹过多时的 Outlook 性能问题](https://docs.microsoft.com/outlook/troubleshoot/performance/performance-issues-if-too-many-items-or-folders)。</span><span class="sxs-lookup"><span data-stu-id="b476b-111">For more information, see [Outlook performance issues when there are too many items or folders in a cached mode .ost or .pst file](https://docs.microsoft.com/outlook/troubleshoot/performance/performance-issues-if-too-many-items-or-folders).</span></span>