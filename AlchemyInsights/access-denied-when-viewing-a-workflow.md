---
title: 查看工作流时访问被拒绝
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: cced887b03876eef527e0166a5a3c9be4b553029
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2019
ms.locfileid: "28277117"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="32798-102">查看工作流时访问被拒绝</span><span class="sxs-lookup"><span data-stu-id="32798-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="32798-103">如果 SharePoint 组的成员的未设置为所有人，带有"访问被拒绝"错误消息可能失败尝试向 SharePoint 组发送电子邮件的 SharePoint 2013 工作流。</span><span class="sxs-lookup"><span data-stu-id="32798-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="32798-104">**若要解决此问题，请执行以下步骤：**</span><span class="sxs-lookup"><span data-stu-id="32798-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="32798-105">允许所有人查看 SharePoint 组的成员。</span><span class="sxs-lookup"><span data-stu-id="32798-105">Allow everybody to see the members of the SharePoint group.</span></span> 
  
 2. <span data-ttu-id="32798-106">移除 SharePoint 组收件人或抄送行的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="32798-106">Remove the SharePoint group from the To or CC line of the email.</span></span> 
  
 3. <span data-ttu-id="32798-107">明确将用户添加到收件人或抄送行如果不能更改 SharePoint 组的成员资格可见。</span><span class="sxs-lookup"><span data-stu-id="32798-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span> 
  
<span data-ttu-id="32798-108">若要查看更多详细信息请参考[HTTP 未经授权到 /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409)。</span><span class="sxs-lookup"><span data-stu-id="32798-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  

