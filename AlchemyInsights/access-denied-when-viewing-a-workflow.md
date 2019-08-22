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
ms.openlocfilehash: 53bd9285e49e220f880eea21923f261302003127
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36495813"
---
# <a name="access-denied-when-viewing-a-workflow"></a>查看工作流时访问被拒绝

如果 SharePoint 组的成员身份未设置为 "所有人", 则尝试向 SharePoint 组发送电子邮件的 SharePoint 2013 工作流可能会失败, 并出现 "访问被拒绝" 错误消息。
  
 **若要解决此问题, 请执行以下步骤:**
  
 1. 允许每个人查看 SharePoint 组的成员。
  
 2. 将 SharePoint 组从电子邮件的 "收件人" 或 "抄送" 行中删除。
  
 3. 如果不能更改 SharePoint 组的成员资格可见性, 请明确地将用户添加到 "收件人" 或 "抄送" 行。
  
若要查看更多详细信息, 请参阅[HTTP 未经授权的/_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409)。
  