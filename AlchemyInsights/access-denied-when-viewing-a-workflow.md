---
title: 查看工作流时访问被拒绝
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 43369c600687d6ac253f70a8535dc2bd0d41687e
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/12/2019
ms.locfileid: "29918816"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="1a94c-102">查看工作流时访问被拒绝</span><span class="sxs-lookup"><span data-stu-id="1a94c-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="1a94c-103">如果 SharePoint 组的成员的未设置为所有人，带有"访问被拒绝"错误消息可能失败尝试向 SharePoint 组发送电子邮件的 SharePoint 2013 工作流。</span><span class="sxs-lookup"><span data-stu-id="1a94c-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="1a94c-104">**若要解决此问题，请执行以下步骤：**</span><span class="sxs-lookup"><span data-stu-id="1a94c-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="1a94c-105">允许所有人查看 SharePoint 组的成员。</span><span class="sxs-lookup"><span data-stu-id="1a94c-105">Allow everybody to see the members of the SharePoint group.</span></span> 
  
 2. <span data-ttu-id="1a94c-106">移除 SharePoint 组收件人或抄送行的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="1a94c-106">Remove the SharePoint group from the To or CC line of the email.</span></span> 
  
 3. <span data-ttu-id="1a94c-107">明确将用户添加到收件人或抄送行如果不能更改 SharePoint 组的成员资格可见。</span><span class="sxs-lookup"><span data-stu-id="1a94c-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span> 
  
<span data-ttu-id="1a94c-108">若要查看更多详细信息请参考[HTTP 未经授权到 /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409)。</span><span class="sxs-lookup"><span data-stu-id="1a94c-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  

