---
title: 查看工作流时访问被拒绝
ms.author: pebaum
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 4ca65583fbd98867026e9e3cc8f36fe38798aa85
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/15/2019
ms.locfileid: "36747738"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="a589b-102">查看工作流时访问被拒绝</span><span class="sxs-lookup"><span data-stu-id="a589b-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="a589b-103">如果 SharePoint 组的成员身份未设置为 "所有人"，则尝试向 SharePoint 组发送电子邮件的 SharePoint 2013 工作流可能会失败，并出现 "访问被拒绝" 错误消息。</span><span class="sxs-lookup"><span data-stu-id="a589b-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="a589b-104">**若要解决此问题，请执行以下步骤：**</span><span class="sxs-lookup"><span data-stu-id="a589b-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="a589b-105">允许每个人查看 SharePoint 组的成员。</span><span class="sxs-lookup"><span data-stu-id="a589b-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="a589b-106">将 SharePoint 组从电子邮件的 "收件人" 或 "抄送" 行中删除。</span><span class="sxs-lookup"><span data-stu-id="a589b-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="a589b-107">如果不能更改 SharePoint 组的成员资格可见性，请明确地将用户添加到 "收件人" 或 "抄送" 行。</span><span class="sxs-lookup"><span data-stu-id="a589b-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="a589b-108">若要查看更多详细信息，请参阅[HTTP 未经授权的/client.svc/sp.utilities.utility.sendemail/_vti_bin](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409)。</span><span class="sxs-lookup"><span data-stu-id="a589b-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  